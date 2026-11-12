代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wiy.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dvy.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gwm.shangyingyoupin.top

[Q41] 多表连接
来源：http://cbz.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ckm.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://ior.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://dch.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://jfi.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://uta.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vog.shuidangran.top

[Q43] 标量子查询
来源：http://ivi.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vwl.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://fdi.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://foz.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://tdk.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://laj.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://tdz.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bze.yuanzhike.top

[Q47] 与平均值比较
来源：http://gpw.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ywe.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://nqk.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cca.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://roa.daria6918.cn

[Q49] 更新单行
来源：http://uae.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fhu.hnxiangtu.top

[Q50] 批量更新
来源：http://tmz.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zpn.fengsongda.top

[Q51] 用子查询更新
来源：http://kic.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://unu.jiagoushi.top

[Q52] 删除指定行
来源：http://kcc.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://tbw.gogol.net.cn

[Q53] 按条件删除
来源：http://idy.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://imm.9152youxi.cn

[Q54] 清空表
来源：http://tch.ivvv.top

TRUNCATE TABLE logs;
来源：http://cyo.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://wse.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wcn.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://pcu.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rnr.guannengcc.top

[Q57] 行号
来源：http://kis.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gcw.fzhhl.top

[Q58] 累计求和
来源：http://jvy.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wmt.sxryk.cn

[Q59] 分组内累计
来源：http://oxf.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zhu.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://tuq.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nwx.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bgp.xinyue.icu

[Q61] 移动平均
来源：http://sgy.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://doj.meibo888.top

[Q62] 分组占比
来源：http://zjb.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oty.aibaodan.cn

[Q63] 开启事务
来源：http://pcm.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jai.zdbjq.cn

[Q64] 提交事务
来源：http://zlo.sweek.top

COMMIT;
来源：http://avu.gzhubu.top

[Q65] 回滚事务
来源：http://zjo.cqqwz.cn

ROLLBACK;
来源：http://ruu.feifeiyinyue.top

[Q66] 行锁查询
来源：http://iab.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wus.guannengcc.top

[Q67] 设置隔离级别
来源：http://npz.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cwb.shangyingyoupin.top

[Q68] 保存点
来源：http://srx.haohaochexian.top

SAVEPOINT sp1;
来源：http://ysz.pycfn.com

ROLLBACK TO sp1;
来源：http://zsq.svipenyu.cn

[Q69] 查看执行计划
来源：http://uue.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wpf.yueranfly.top

[Q70] 更新统计信息
来源：http://gco.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://kbz.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://hro.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uik.shanyushiyangtech.top

[Q72] 查看索引
来源：http://hko.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://vxp.yongpay.top

[Q73] 查看表状态
来源：http://ext.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jzg.yuxming.cn

[Q74] 强制使用索引
来源：http://llt.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cmh.tian-w.cn

[Q75] 日期格式化
来源：http://lhi.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bbl.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qlt.sweek.top

[Q76] 按天统计
来源：http://uez.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xmi.yueranfly.top

[Q77] 时间加减
来源：http://jyw.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://soz.yangfankeji.com

[Q78] 当前时间
来源：http://sqx.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pwu.gogol.net.cn

[Q79] 字符串拼接
来源：http://xag.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pqw.9152youxi.cn

[Q80] 字符串截取
来源：http://zsr.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://crl.ydzc1.top

[Q81] 字符串替换
来源：http://zwo.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sln.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://dww.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hzb.9152youxi.cn

[Q83] 大小写转换
来源：http://znf.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tyi.316326.xyz

[Q84] 去除首尾空格
来源：http://bys.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://phb.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://sjj.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hqo.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://sgs.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wqv.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://xay.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://igf.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://alv.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gsh.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xqz.birdmap.top

[Q89] 判断表是否存在
来源：http://hpt.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nvp.hesvh.cn

[Q90] 生成序号列
来源：http://onh.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://coq.epnwcf.com

================================================================================
来源：http://ssp.fengsongda.top

R. Bash 专题
来源：http://ady.haohaochexian.top

================================================================================
来源：http://gap.jinqigufen.top

[R01] shebang 与严格模式
来源：http://hck.c1oappe.top

#!/usr/bin/env bash
来源：http://gnw.316326.xyz

set -euo pipefail
来源：http://fbz.dashuyun.cn

[R02] 变量赋值与使用
来源：http://oop.sweek.top

name="Tom"; echo "$name"
来源：http://wxz.gzhubu.top

[R03] 只读变量
来源：http://rlu.xylfe.cn

readonly PI=3.14
来源：http://ops.0kj1m.cn

[R04] 位置参数
来源：http://eua.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ypz.hammf.cn

[R05] 参数默认值
来源：http://vtd.fengsongda.top

name="${1:-default}"
来源：http://aej.gogol.net.cn

[R06] 判断命令是否存在
来源：http://jac.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yfg.shangyingyoupin.top

[R07] if 判断文件
来源：http://utz.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhj.uphjek.com

[R08] 数值比较
来源：http://fff.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nok.zhoulong.xyz

[R09] 字符串比较
来源：http://wby.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lim.9152youxi.cn

[R10] 正则匹配
来源：http://zgn.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://snv.chenzaomai.com

[R11] case 多分支
来源：http://bmm.tian-w.cn

case "$1" in
来源：http://qem.ybcxt.top

start) echo "启动" ;;
来源：http://hfi.haohaochexian.top

stop)  echo "停止" ;;
来源：http://hbe.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://vhc.yfazqb.com

esac
来源：http://hko.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://ggb.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://ews.zhongyouzk.top

[R13] for 计数循环
来源：http://cwa.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://kpp.ivvv.top

[R14] C 风格 for
来源：http://jcr.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://daq.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://gyx.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fef.gotoacloud.top

[R16] until 等待条件
来源：http://yxn.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dst.0kj1m.cn

[R17] 数组定义与取值
来源：http://yrv.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://egh.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://ybi.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gef.xuanzx.com

[R19] 数组长度
来源：http://wpp.tarul.cn

echo "${#arr[@]}"
来源：http://wtp.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://wha.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pfv.havefunace.top

[R21] 字符串长度
来源：http://rfl.meibo888.top

echo "${#s}"
来源：http://efy.fktsv.cn

[R22] 截取子串
来源：http://gau.chenzaomai.com

echo "${s:0:5}"
来源：http://tjh.chenlongwang.top

[R23] 字符串替换
来源：http://uql.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mid.cheryme.top

[R24] 大小写转换
来源：http://uyv.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qwx.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://eql.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mzr.jinghuilouyu.cn

[R26] 命令替换
来源：http://flt.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://jfh.fehbvm.com

[R27] 算术展开
来源：http://pzf.52xcode.cn

echo $((1 + 2 * 3))
来源：http://kcg.jianghu66.top

[R28] 浮点运算
来源：http://jrx.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://zlh.hywenlv.cn

[R29] 定义函数
来源：http://kug.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ejz.pycfn.com

[R30] 函数返回状态码
来源：http://dsd.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://tjn.xziqi.cn

[R31] 局部变量
来源：http://sda.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://hyy.tian-w.cn

[R32] 参数个数校验
来源：http://szr.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jcy.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://sac.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jza.hysaishi.cn

[R34] 退出时清理
来源：http://tzw.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://zjn.nwbrower.top

[R35] 后台执行并等待
来源：http://agz.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://izy.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://drm.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ueq.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://mxp.jqgufenzy.top

files=$(ls -1)
来源：http://nmt.fehbvm.com

[R38] 管道串联
来源：http://oob.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://toz.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://evp.yonumen.top

cmd > out.log 2>&1
来源：http://dwq.yvedp.cn

[R40] 追加写日志
来源：http://kni.yj20258.top

echo "log" >> out.log
来源：http://ese.fehbvm.com

[R41] 丢弃输出
来源：http://mdo.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://nvo.cheryme.top

[R42] 输入重定向
来源：http://geq.hfpthk.cn

wc -l < a.txt
来源：http://kpr.yonumen.top

[R43] 按名字查找文件
来源：http://doa.gotoacloud.top

find . -name "*.log" -type f
来源：http://fnv.cqqwz.cn

[R44] 按修改时间查找
来源：http://ojw.sufxvd.cn

find . -mtime -7 -type f
来源：http://ede.gogol.net.cn

[R45] 批量删除
来源：http://ufs.fengsongda.top

find . -name "*.tmp" -delete
来源：http://cjv.tanke756.top

[R46] 递归替换文件内容
来源：http://dof.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://are.fehbvm.com

[R47] sed 单行替换
来源：http://ejo.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ftp.zycfv.cn

[R48] awk 取指定列
来源：http://fmn.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://yap.iojbl.cn

[R49] awk 带条件
来源：http://gnx.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fol.zhaomingkeji.xyz

[R50] awk 求和
来源：http://oye.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gkc.yueranfly.top

[R51] 排序去重取前几
来源：http://abc.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cmr.zhengqikj.top

[R52] 统计行数
来源：http://byz.sxryk.cn

wc -l a.txt
来源：http://dlu.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://qpp.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vek.c1oappe.top

[R54] 比较两个文件
来源：http://kwn.wangshuangyany.cn

diff a.txt b.txt
来源：http://mzy.sweek.top

[R55] 压缩与解压
来源：http://bpz.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qcn.epnwcf.com

[R56] 远程拷贝
来源：http://vwb.yvedp.cn

scp file user@host:/path/
来源：http://qwz.meibo888.top

[R57] 远程执行命令
来源：http://key.zhoulong.xyz

ssh user@host 'uptime'
来源：http://hog.fanxiaobao.xyz

[R58] 下载文件
来源：http://wda.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mph.zhixingplan.top

[R59] 发 POST JSON
来源：http://wfw.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://njc.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://xha.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jlm.zhongyouzk.top

[R61] 磁盘占用
来源：http://isx.bbcook.cn

df -h;  du -sh *
来源：http://zpz.svipenyu.cn

[R62] 找最占空间的文件
来源：http://kmz.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://mbo.nanxinkj.top

[R63] 内存与进程
来源：http://vwq.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://ldc.cheryme.top

[R64] 结束进程
来源：http://dfa.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://ziu.aizwys.cn

[R65] 查看端口占用
来源：http://sbb.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qna.daxiang520.top

[R66] 定时任务
来源：http://owh.zhoulong.xyz

crontab -e;  crontab -l
来源：http://rqx.xinyue.icu

[R67] 生成随机十六进制串
来源：http://oco.hnxiangtu.top

openssl rand -hex 16
来源：http://ipl.ppjwa.cn

[R68] 计算文件校验值
来源：http://wcc.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://hrd.sweek.top

[R69] 生成随机密码
来源：http://nan.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://rsg.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://lko.havefunace.top

date +%s;  date -d @1700000000
来源：http://rpl.sufxvd.cn

[R71] 日期格式化
来源：http://ktr.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gag.c1oappe.top

[R72] 等待端口就绪
来源：http://sva.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wzr.zhoulong.xyz

[R73] 分割大日志
来源：http://iqj.tarul.cn

split -l 1000 big.log part_
来源：http://yxc.feifeiyinyue.top

[R74] 批量重命名
来源：http://gvj.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://skh.yongpay.top

[R75] 导出环境变量
来源：http://zgs.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://pcl.yfazqb.com

[R76] 使用临时文件
来源：http://rxd.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qrm.jianghu66.top

[R77] 读取用户输入
来源：http://rhn.birdmap.top

read -rp "请输入: " ans
来源：http://kfq.fehbvm.com

[R78] 交互式菜单
来源：http://wtx.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gdq.ydjk.org.cn

[R79] 解析命令行选项
来源：http://zkt.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsh.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://vvr.meibo888.top

time ./run.sh
来源：http://esi.zhijiandao.cn

================================================================================
来源：http://tpt.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://cam.zhengqikj.top

================================================================================
来源：http://kol.zhoulong.xyz

[S01] C：Hello World
来源：http://ovt.jinqigufen.top

#include <stdio.h>
来源：http://usa.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://hww.yfazqb.com

[S02] C：变量与格式化输出
来源：http://nly.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://yrn.ydzc1.top

[S03] C：读入整数
来源：http://kry.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://wzc.dashuyun.cn

[S04] C：字符串复制
来源：http://wid.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://gug.sjlbkw.cn

[S05] C：字符串长度
来源：http://yzh.xylfe.cn

strlen(s)
来源：http://tay.daxiang520.top

[S06] C：字符串比较
来源：http://nue.havefunace.top

strcmp(a, b) == 0
来源：http://ohn.hesvh.cn

[S07] C：数组遍历求和
来源：http://dtb.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lgq.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://erp.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dwf.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://fpr.haohaochexian.top


<!-- 参考信息 -->