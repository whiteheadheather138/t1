代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://uot.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://cot.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://zuz.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://khp.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://wnr.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dpy.bbcook.cn

[Q43] 标量子查询
来源：http://jxu.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hyf.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://wqd.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cuz.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://lwp.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ius.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://ocq.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ted.vqdsnc.cn

[Q47] 与平均值比较
来源：http://peu.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xfc.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://lgi.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mzn.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://eeo.dashuyun.cn

[Q49] 更新单行
来源：http://onb.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rcb.chenjidiqi.icu

[Q50] 批量更新
来源：http://xvp.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ain.tarul.cn

[Q51] 用子查询更新
来源：http://ayh.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mau.feifeiyinyue.top

[Q52] 删除指定行
来源：http://axe.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://ooo.haohaochexian.top

[Q53] 按条件删除
来源：http://pds.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kev.fanxiaobao.xyz

[Q54] 清空表
来源：http://rnb.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://neg.uphjek.com

[Q55] 排名（并列占位）
来源：http://lkp.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pae.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://uzx.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kkc.yuanzhike.top

[Q57] 行号
来源：http://yvk.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uli.zhiwuduotai.top

[Q58] 累计求和
来源：http://nbl.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dmf.xylfe.cn

[Q59] 分组内累计
来源：http://qbm.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vno.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://mmq.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ikx.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lyq.andypj.xyz

[Q61] 移动平均
来源：http://tsn.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ojh.ivvv.top

[Q62] 分组占比
来源：http://qyg.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xqc.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://ibu.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sut.mhx1999.top

[Q64] 提交事务
来源：http://nly.uphjek.com

COMMIT;
来源：http://uku.9152youxi.cn

[Q65] 回滚事务
来源：http://lbc.daria6918.cn

ROLLBACK;
来源：http://big.zhiwuduotai.top

[Q66] 行锁查询
来源：http://rxn.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sbi.hysaishi.cn

[Q67] 设置隔离级别
来源：http://qru.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsi.svipenyu.cn

[Q68] 保存点
来源：http://nur.gotoacloud.top

SAVEPOINT sp1;
来源：http://chm.daria6918.cn

ROLLBACK TO sp1;
来源：http://clx.hnqzz.top

[Q69] 查看执行计划
来源：http://frf.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mys.yuanzhike.top

[Q70] 更新统计信息
来源：http://wbq.jinqigufen.top

ANALYZE TABLE users;
来源：http://odv.ybcxt.top

[Q71] 查看建表语句
来源：http://jym.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hqn.ybcxt.top

[Q72] 查看索引
来源：http://bcc.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://jul.zhengqikj.top

[Q73] 查看表状态
来源：http://wak.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://whs.zycfv.cn

[Q74] 强制使用索引
来源：http://bin.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rig.yj20258888.top

[Q75] 日期格式化
来源：http://lfl.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vpa.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oto.jlsjyb.cn

[Q76] 按天统计
来源：http://tzj.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iyx.kuanghao11.cn

[Q77] 时间加减
来源：http://yee.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tpn.gzhubu.top

[Q78] 当前时间
来源：http://unz.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lkk.redwolf501.top

[Q79] 字符串拼接
来源：http://iae.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ilp.52xcode.cn

[Q80] 字符串截取
来源：http://ohd.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://htb.daxiang520.top

[Q81] 字符串替换
来源：http://qke.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lgu.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://kpi.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xtj.zhoulong.xyz

[Q83] 大小写转换
来源：http://lrw.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://llq.yj202588.top

[Q84] 去除首尾空格
来源：http://diz.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://iwz.yj20258.top

[Q85] 数值取整
来源：http://eex.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ddl.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://sqq.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rmj.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://vcv.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ppz.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://vpi.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ick.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ewt.daria6918.cn

[Q89] 判断表是否存在
来源：http://hcf.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ewm.fktsv.cn

[Q90] 生成序号列
来源：http://xoh.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lcl.zycfv.cn

================================================================================
来源：http://jmg.xziqi.cn

R. Bash 专题
来源：http://zjz.zdbjq.cn

================================================================================
来源：http://ijp.epnwcf.com

[R01] shebang 与严格模式
来源：http://pht.gogol.net.cn

#!/usr/bin/env bash
来源：http://aue.snrcjt.cn

set -euo pipefail
来源：http://zni.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://osp.vehdjk.com

name="Tom"; echo "$name"
来源：http://yws.xuanzx.com

[R03] 只读变量
来源：http://uft.zhongyouzk.top

readonly PI=3.14
来源：http://vzo.wangshuangyany.cn

[R04] 位置参数
来源：http://xpa.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fbp.nwbrower.top

[R05] 参数默认值
来源：http://fyb.wangshuangyany.cn

name="${1:-default}"
来源：http://zgs.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://wqe.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gay.cqqwz.cn

[R07] if 判断文件
来源：http://ojc.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qyq.hcnkem.com

[R08] 数值比较
来源：http://ccx.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ief.fktsv.cn

[R09] 字符串比较
来源：http://yue.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://juw.c1oappe.top

[R10] 正则匹配
来源：http://ztr.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vfu.cucudq.cn

[R11] case 多分支
来源：http://ujx.0kj1m.cn

case "$1" in
来源：http://snp.dianchejie.cn

start) echo "启动" ;;
来源：http://ygt.birdmap.top

stop)  echo "停止" ;;
来源：http://kgn.redwolf501.top

*)     echo "未知命令" ;;
来源：http://pqg.zhaomingkeji.xyz

esac
来源：http://xcz.zycfv.cn

[R12] for 遍历文件
来源：http://yro.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://odu.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://das.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://txp.hnqzz.top

[R14] C 风格 for
来源：http://air.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kla.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://ezc.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mdo.sufxvd.cn

[R16] until 等待条件
来源：http://yhk.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bbd.zhoulong.xyz

[R17] 数组定义与取值
来源：http://jla.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://ltq.shangyingyoupin.top

[R18] 遍历数组
来源：http://czw.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wwm.haohaochexian.top

[R19] 数组长度
来源：http://eok.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://rwb.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://xwo.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qdi.uphjek.com

[R21] 字符串长度
来源：http://nos.feifeiyinyue.top

echo "${#s}"
来源：http://cqn.iojbl.cn

[R22] 截取子串
来源：http://gjz.iojbl.cn

echo "${s:0:5}"
来源：http://yrk.guowangkeji.top

[R23] 字符串替换
来源：http://qfc.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ufn.birdmap.top

[R24] 大小写转换
来源：http://zlo.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://aas.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://zbf.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://acf.dashuyun.cn

[R26] 命令替换
来源：http://tcn.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://qrd.wangshuangyany.cn

[R27] 算术展开
来源：http://izr.mhx1999.top

echo $((1 + 2 * 3))
来源：http://cxk.haohaochexian.top

[R28] 浮点运算
来源：http://pvd.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://pzm.sufxvd.cn

[R29] 定义函数
来源：http://nks.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://arc.gotoacloud.top

[R30] 函数返回状态码
来源：http://zjf.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://aow.gzhubu.top

[R31] 局部变量
来源：http://aqy.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://sey.aizwys.cn

[R32] 参数个数校验
来源：http://ubw.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kfk.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://kdq.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dhn.wangshuangyany.cn

[R34] 退出时清理
来源：http://asj.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://ulb.sxryk.cn

[R35] 后台执行并等待
来源：http://wxk.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kdm.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://rig.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkm.nanxinkj.top

[R37] 把输出赋给变量
来源：http://wxc.jqgufenzy.top

files=$(ls -1)
来源：http://qeu.c1oappe.top

[R38] 管道串联
来源：http://svi.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://jix.hammf.cn

[R39] 重定向标准输出与错误
来源：http://yeu.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://vdh.cheryme.top

[R40] 追加写日志
来源：http://yie.gotoacloud.top

echo "log" >> out.log
来源：http://iwh.jinqigfzy.top

[R41] 丢弃输出
来源：http://bwp.yonumen.top

cmd >/dev/null 2>&1
来源：http://jpg.dashuyun.cn

[R42] 输入重定向
来源：http://vkw.ivvv.top

wc -l < a.txt
来源：http://fdq.sxryk.cn

[R43] 按名字查找文件
来源：http://yal.epnwcf.com

find . -name "*.log" -type f
来源：http://xxc.jinqigufen.top

[R44] 按修改时间查找
来源：http://ugi.tian-w.cn

find . -mtime -7 -type f
来源：http://dww.xylfe.cn

[R45] 批量删除
来源：http://rcy.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://utn.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://yrs.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oay.tianlin.xyz

[R47] sed 单行替换
来源：http://jzx.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kiz.jqgfzy.top

[R48] awk 取指定列
来源：http://rgb.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://qzx.tianlin.xyz

[R49] awk 带条件
来源：http://kmi.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vkm.ehwqpu.com

[R50] awk 求和
来源：http://ueg.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sax.jqgufenzy.top

[R51] 排序去重取前几
来源：http://dxa.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://mrj.sufxvd.cn

[R52] 统计行数
来源：http://cza.vehdjk.com

wc -l a.txt
来源：http://lxf.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://cvd.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tee.fengsongda.top

[R54] 比较两个文件
来源：http://bts.shuidangran.top

diff a.txt b.txt
来源：http://uwo.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://dxr.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ydc.xylfe.cn

[R56] 远程拷贝
来源：http://teu.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://onr.xylfe.cn

[R57] 远程执行命令
来源：http://zyu.vehdjk.com

ssh user@host 'uptime'
来源：http://oos.daria6918.cn

[R58] 下载文件
来源：http://crl.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydt.guowangkeji.top

[R59] 发 POST JSON
来源：http://ded.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jwu.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://gjc.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kkj.feifeiyinyue.top

[R61] 磁盘占用
来源：http://plu.kuanghao11.cn

df -h;  du -sh *
来源：http://etj.aizwys.cn

[R62] 找最占空间的文件
来源：http://lgo.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://lqc.guannengcc.top

[R63] 内存与进程
来源：http://rzc.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://gcw.hongshengwenyu.top

[R64] 结束进程
来源：http://jtw.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://gld.gaohongyu789.top

[R65] 查看端口占用
来源：http://dxf.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mzu.cheryme.top

[R66] 定时任务
来源：http://yfg.gotoacloud.top

crontab -e;  crontab -l
来源：http://dlx.tian-w.cn

[R67] 生成随机十六进制串
来源：http://iot.pycfn.com

openssl rand -hex 16
来源：http://qoz.bbcook.cn

[R68] 计算文件校验值
来源：http://swn.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://qhd.sufxvd.cn

[R69] 生成随机密码
来源：http://dlw.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://qpk.yvedp.cn

[R70] 时间戳与互转
来源：http://gcw.yongpay.top

date +%s;  date -d @1700000000
来源：http://hvz.vqdsnc.cn

[R71] 日期格式化
来源：http://zdc.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://nwy.zhengqikj.top

[R72] 等待端口就绪
来源：http://zlm.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dvv.tanke756.top

[R73] 分割大日志
来源：http://hbl.xinyue.icu

split -l 1000 big.log part_
来源：http://kqd.mhx1999.top

[R74] 批量重命名
来源：http://cmf.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ryj.ydjk.org.cn

[R75] 导出环境变量
来源：http://ape.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://kyf.jlsjyb.cn

[R76] 使用临时文件
来源：http://qzl.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vyi.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://oob.tanke756.top

read -rp "请输入: " ans
来源：http://jcp.yfazqb.com

[R78] 交互式菜单
来源：http://lrp.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eop.316326.xyz

[R79] 解析命令行选项
来源：http://oiw.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://djg.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://maf.sysykeji.top

time ./run.sh
来源：http://uda.xylfe.cn

================================================================================
来源：http://osb.yj20258.top

S. C / C++ 专题
来源：http://ids.shzxlz.cn

================================================================================
来源：http://zhj.hongshengwenyu.top

[S01] C：Hello World
来源：http://gqx.cashguo.top

#include <stdio.h>
来源：http://gih.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qqp.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://jey.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://ssh.birdmap.top

[S03] C：读入整数
来源：http://fma.meibo888.top

int x; scanf("%d", &x);
来源：http://ysw.chenlongwang.top

[S04] C：字符串复制
来源：http://hvf.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://rhk.sjlbkw.cn

[S05] C：字符串长度
来源：http://qpg.mhx1999.top

strlen(s)
来源：http://iuj.jlsjyb.cn

[S06] C：字符串比较
来源：http://grg.ydzc1.top

strcmp(a, b) == 0
来源：http://hjn.havefunace.top

[S07] C：数组遍历求和
来源：http://hje.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pjl.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://xcn.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lqw.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://nff.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lhr.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://lwj.bjfxy.top

int *p = &a;  *p = 5;
来源：http://ybz.zhoulong.xyz

[S11] C：逐行读文件
来源：http://msv.tanke756.top


<!-- 参考信息 -->