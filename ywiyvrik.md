代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://zps.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://ebh.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://uxx.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://upl.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://hcn.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ljp.yangfankeji.com

[Q43] 标量子查询
来源：http://xkp.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cax.mhx1999.top

[Q44] IN 子查询
来源：http://mal.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aig.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://ujl.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cke.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://noy.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qvm.chenlongwang.top

[Q47] 与平均值比较
来源：http://lfk.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gem.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://yjr.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rvv.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hru.ppjwa.cn

[Q49] 更新单行
来源：http://vvu.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ymf.haohaochexian.top

[Q50] 批量更新
来源：http://oev.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gyo.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://pmt.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tkp.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://wgd.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://xcz.zhiwuduotai.top

[Q53] 按条件删除
来源：http://ikz.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://igi.fengsongda.top

[Q54] 清空表
来源：http://yrk.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://nvk.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://odc.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vjv.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://ums.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjg.c1oappe.top

[Q57] 行号
来源：http://hal.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://chl.vehdjk.com

[Q58] 累计求和
来源：http://yuz.nanxinkj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cvg.9152youxi.cn

[Q59] 分组内累计
来源：http://jeq.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://typ.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://hmb.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ygj.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rnv.havefunace.top

[Q61] 移动平均
来源：http://dpj.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ely.nwbrower.top

[Q62] 分组占比
来源：http://xsz.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ags.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://ypm.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jck.mhx1999.top

[Q64] 提交事务
来源：http://jee.sweek.top

COMMIT;
来源：http://gkx.c1oappe.top

[Q65] 回滚事务
来源：http://fpb.sxryk.cn

ROLLBACK;
来源：http://evg.tanke756.top

[Q66] 行锁查询
来源：http://nsu.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fah.wangdashe.top

[Q67] 设置隔离级别
来源：http://ayp.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mon.zhongyouzk.top

[Q68] 保存点
来源：http://mbt.hywenlv.cn

SAVEPOINT sp1;
来源：http://wlh.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://wqc.snrcjt.cn

[Q69] 查看执行计划
来源：http://nlo.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dtd.jianghu66.top

[Q70] 更新统计信息
来源：http://vyy.yuanzhike.top

ANALYZE TABLE users;
来源：http://nhv.hywenlv.cn

[Q71] 查看建表语句
来源：http://amy.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ape.chenzaomai.com

[Q72] 查看索引
来源：http://prj.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://fhc.yvedp.cn

[Q73] 查看表状态
来源：http://toq.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mvu.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://ymp.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mqa.vehdjk.com

[Q75] 日期格式化
来源：http://mxw.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://goz.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bxs.fktsv.cn

[Q76] 按天统计
来源：http://ixi.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gpp.shuidangran.top

[Q77] 时间加减
来源：http://zco.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://msq.sweek.top

[Q78] 当前时间
来源：http://qyq.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ztw.nanxinkj.top

[Q79] 字符串拼接
来源：http://cxr.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yzd.tianlin.xyz

[Q80] 字符串截取
来源：http://uxj.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kqd.zhixingplan.top

[Q81] 字符串替换
来源：http://rih.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hoz.yonumen.top

[Q82] 字符长度与字节长度
来源：http://ktw.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://egc.9152youxi.cn

[Q83] 大小写转换
来源：http://iri.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oze.cheryme.top

[Q84] 去除首尾空格
来源：http://juv.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://nvv.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://xud.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lyd.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://jny.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mkj.cucudq.cn

[Q87] JSON 字段做条件
来源：http://hwz.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pon.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://tuk.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dsa.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ydp.shzxlz.cn

[Q89] 判断表是否存在
来源：http://dpg.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ehz.wangdashe.top

[Q90] 生成序号列
来源：http://ezv.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yjv.zycfv.cn

================================================================================
来源：http://ppl.fehbvm.com

R. Bash 专题
来源：http://sts.iojbl.cn

================================================================================
来源：http://ieu.gotoacloud.top

[R01] shebang 与严格模式
来源：http://pgr.andypj.xyz

#!/usr/bin/env bash
来源：http://pgi.pycfn.com

set -euo pipefail
来源：http://ohp.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://jtv.ehwqpu.com

name="Tom"; echo "$name"
来源：http://quq.shanyushiyangtech.top

[R03] 只读变量
来源：http://jeo.tarul.cn

readonly PI=3.14
来源：http://uvv.zycfv.cn

[R04] 位置参数
来源：http://dcn.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ice.yj202588.top

[R05] 参数默认值
来源：http://abt.9152youxi.cn

name="${1:-default}"
来源：http://maw.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://rfp.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pxn.ivvv.top

[R07] if 判断文件
来源：http://cka.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lvx.nanxinkj.top

[R08] 数值比较
来源：http://tso.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://erh.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://rll.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://die.hesvh.cn

[R10] 正则匹配
来源：http://fne.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qcj.9152youxi.cn

[R11] case 多分支
来源：http://tcu.zhijiandao.cn

case "$1" in
来源：http://yqa.zhongyouzk.top

start) echo "启动" ;;
来源：http://icg.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://gdf.daxiang520.top

*)     echo "未知命令" ;;
来源：http://bku.sweek.top

esac
来源：http://mot.jqgfzy.top

[R12] for 遍历文件
来源：http://cls.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://srn.zhixingplan.top

[R13] for 计数循环
来源：http://kdw.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://flm.tian-w.cn

[R14] C 风格 for
来源：http://fsx.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wbt.hysaishi.cn

[R15] while 逐行读文件
来源：http://gcx.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://icy.aibaodan.cn

[R16] until 等待条件
来源：http://axp.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gui.vqdsnc.cn

[R17] 数组定义与取值
来源：http://tjx.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fyu.0kj1m.cn

[R18] 遍历数组
来源：http://htv.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qiq.epnwcf.com

[R19] 数组长度
来源：http://hsr.aizwys.cn

echo "${#arr[@]}"
来源：http://iob.gogol.net.cn

[R20] 关联数组（字典）
来源：http://jjr.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uqd.yongpay.top

[R21] 字符串长度
来源：http://mcz.jlsjyb.cn

echo "${#s}"
来源：http://kql.zhaomingkeji.xyz

[R22] 截取子串
来源：http://ghi.yangfankeji.com

echo "${s:0:5}"
来源：http://rjc.fzhhl.top

[R23] 字符串替换
来源：http://tzt.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://caf.jinghuilouyu.cn

[R24] 大小写转换
来源：http://osn.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://vgi.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://yhn.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://amw.smart0.xyz

[R26] 命令替换
来源：http://kdy.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://lpf.chenzaomai.com

[R27] 算术展开
来源：http://qwz.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://eyc.sufxvd.cn

[R28] 浮点运算
来源：http://cxi.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://xai.jinyuanbaomall.cn

[R29] 定义函数
来源：http://imw.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezj.tian-w.cn

[R30] 函数返回状态码
来源：http://dhf.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://cuz.shzxlz.cn

[R31] 局部变量
来源：http://mje.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://gar.chenlongwang.top

[R32] 参数个数校验
来源：http://qbs.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jtj.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://bsn.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qmt.jinqigfzy.top

[R34] 退出时清理
来源：http://ioj.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://kvk.chenlongwang.top

[R35] 后台执行并等待
来源：http://ydv.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://upx.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://yht.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uce.hfpthk.cn

[R37] 把输出赋给变量
来源：http://cpz.shzxlz.cn

files=$(ls -1)
来源：http://inf.hfpthk.cn

[R38] 管道串联
来源：http://yns.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://xiq.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://brk.daxiang520.top

cmd > out.log 2>&1
来源：http://hhl.ppjwa.cn

[R40] 追加写日志
来源：http://zpv.jyoumei.cn

echo "log" >> out.log
来源：http://isa.zhiwuduotai.top

[R41] 丢弃输出
来源：http://baw.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://bxo.gzhubu.top

[R42] 输入重定向
来源：http://odz.yfazqb.com

wc -l < a.txt
来源：http://okf.hysaishi.cn

[R43] 按名字查找文件
来源：http://ekh.redwolf501.top

find . -name "*.log" -type f
来源：http://qik.svipenyu.cn

[R44] 按修改时间查找
来源：http://ogs.cheryme.top

find . -mtime -7 -type f
来源：http://csb.chenlongwang.top

[R45] 批量删除
来源：http://ivs.fehbvm.com

find . -name "*.tmp" -delete
来源：http://xeg.hfpthk.cn

[R46] 递归替换文件内容
来源：http://jch.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://phh.aizwys.cn

[R47] sed 单行替换
来源：http://nxl.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://irr.vqdsnc.cn

[R48] awk 取指定列
来源：http://fhk.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://anc.daria6918.cn

[R49] awk 带条件
来源：http://rwh.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jjm.yuanzhike.top

[R50] awk 求和
来源：http://qcm.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://mgr.yuxming.cn

[R51] 排序去重取前几
来源：http://xos.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dtk.cucudq.cn

[R52] 统计行数
来源：http://qwb.ctjpmb.com

wc -l a.txt
来源：http://dgw.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://eap.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zcw.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://ezd.dashuyun.cn

diff a.txt b.txt
来源：http://kft.guannengcc.top

[R55] 压缩与解压
来源：http://upf.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rsl.pycfn.com

[R56] 远程拷贝
来源：http://xsx.vehdjk.com

scp file user@host:/path/
来源：http://tgn.shangyingyoupin.top

[R57] 远程执行命令
来源：http://pam.nanxuanxn.top

ssh user@host 'uptime'
来源：http://blx.hcnkem.com

[R58] 下载文件
来源：http://yqh.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://owa.smart0.xyz

[R59] 发 POST JSON
来源：http://ocy.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nuh.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://pjh.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pgd.shzxlz.cn

[R61] 磁盘占用
来源：http://ckf.jqgufenzy.top

df -h;  du -sh *
来源：http://szz.gzhubu.top

[R62] 找最占空间的文件
来源：http://qsi.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://aco.xuanzx.com

[R63] 内存与进程
来源：http://rzu.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://ytt.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://mqu.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://fmn.feifeiyinyue.top

[R65] 查看端口占用
来源：http://gar.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfo.zhijiandao.cn

[R66] 定时任务
来源：http://woa.jiagoushi.top

crontab -e;  crontab -l
来源：http://zpl.nwbrower.top

[R67] 生成随机十六进制串
来源：http://avx.smart0.xyz

openssl rand -hex 16
来源：http://txi.ydzc1.top

[R68] 计算文件校验值
来源：http://ojo.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://osw.yvedp.cn

[R69] 生成随机密码
来源：http://ukj.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://csn.yonumen.top

[R70] 时间戳与互转
来源：http://hzg.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://mls.sjlbkw.cn

[R71] 日期格式化
来源：http://mrv.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fib.sysykeji.top

[R72] 等待端口就绪
来源：http://ahr.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yhv.aibaodan.cn

[R73] 分割大日志
来源：http://byv.xylfe.cn

split -l 1000 big.log part_
来源：http://ksw.guowangkeji.top

[R74] 批量重命名
来源：http://pgt.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rft.sxryk.cn

[R75] 导出环境变量
来源：http://rna.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://may.yj202588.top

[R76] 使用临时文件
来源：http://hxt.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kft.xuetiantiany.cn

[R77] 读取用户输入
来源：http://lbc.jqgfzy.top

read -rp "请输入: " ans
来源：http://iuv.jqgfzy.top

[R78] 交互式菜单
来源：http://pjk.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qet.yuanzhike.top

[R79] 解析命令行选项
来源：http://rtp.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bvn.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://cxy.cucudq.cn

time ./run.sh
来源：http://ckg.zdqjudy.top

================================================================================
来源：http://sml.ivvv.top

S. C / C++ 专题
来源：http://tvm.hnxiangtu.top

================================================================================
来源：http://sip.shanyushiyangtech.top

[S01] C：Hello World
来源：http://wxa.c1oappe.top

#include <stdio.h>
来源：http://unj.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ipc.ybcxt.top

[S02] C：变量与格式化输出
来源：http://uol.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://fyj.gaohongyu789.top

[S03] C：读入整数
来源：http://scp.hywenlv.cn

int x; scanf("%d", &x);
来源：http://vgl.52xcode.cn

[S04] C：字符串复制
来源：http://pkg.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://spl.xziqi.cn

[S05] C：字符串长度
来源：http://zee.sjlbkw.cn

strlen(s)
来源：http://che.zhongyouzk.top

[S06] C：字符串比较
来源：http://erk.birdmap.top

strcmp(a, b) == 0
来源：http://fkr.zycfv.cn

[S07] C：数组遍历求和
来源：http://qzd.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hhx.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://ayv.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iik.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://soe.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kxn.sjlbkw.cn

[S10] C：指针与解引用
来源：http://kfv.nwbrower.top

int *p = &a;  *p = 5;
来源：http://dmn.pycfn.com

[S11] C：逐行读文件
来源：http://mrz.hesvh.cn


<!-- 参考信息 -->