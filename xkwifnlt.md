代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tel.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nqp.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pwf.tian-w.cn

[Q41] 多表连接
来源：http://qnf.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fxw.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://jhi.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://kmw.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://mey.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://vfy.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gag.fzhhl.top

[Q43] 标量子查询
来源：http://dqx.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dgc.yuxming.cn

[Q44] IN 子查询
来源：http://kcl.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fze.yj20258.top

[Q45] EXISTS 判断存在
来源：http://evm.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wtj.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://nyw.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bqm.daxiang520.top

[Q47] 与平均值比较
来源：http://flf.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lmd.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://ysh.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dwm.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://ekg.zdbjq.cn

[Q49] 更新单行
来源：http://lze.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwd.9152youxi.cn

[Q50] 批量更新
来源：http://goy.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://olm.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://bdg.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eol.gzhubu.top

[Q52] 删除指定行
来源：http://xfq.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://xqg.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://ptf.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nvf.dashuyun.cn

[Q54] 清空表
来源：http://ffd.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://sbz.sysykeji.top

[Q55] 排名（并列占位）
来源：http://rsi.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gpu.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://jtk.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vro.gaohongyu789.top

[Q57] 行号
来源：http://jhw.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pce.sweek.top

[Q58] 累计求和
来源：http://ngv.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mxp.shuidangran.top

[Q59] 分组内累计
来源：http://uwu.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pvt.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://wot.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ynr.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kof.daxiang520.top

[Q61] 移动平均
来源：http://zwo.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sbf.sxryk.cn

[Q62] 分组占比
来源：http://rjz.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eml.hywenlv.cn

[Q63] 开启事务
来源：http://zwg.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fei.cqqwz.cn

[Q64] 提交事务
来源：http://jvc.zdbjq.cn

COMMIT;
来源：http://ysu.wangshuangyany.cn

[Q65] 回滚事务
来源：http://eav.shuidangran.top

ROLLBACK;
来源：http://iac.fzhhl.top

[Q66] 行锁查询
来源：http://ujh.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nsg.ehwqpu.com

[Q67] 设置隔离级别
来源：http://tzu.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ybt.fzhhl.top

[Q68] 保存点
来源：http://tga.c1oappe.top

SAVEPOINT sp1;
来源：http://owd.tian-w.cn

ROLLBACK TO sp1;
来源：http://vhy.cucudq.cn

[Q69] 查看执行计划
来源：http://efs.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ncc.jianghu66.top

[Q70] 更新统计信息
来源：http://jqz.zhongyouzk.top

ANALYZE TABLE users;
来源：http://unn.c1oappe.top

[Q71] 查看建表语句
来源：http://ykr.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yro.zhongyouzk.top

[Q72] 查看索引
来源：http://daf.zhengqikj.top

SHOW INDEX FROM users;
来源：http://tgt.wangshuangyany.cn

[Q73] 查看表状态
来源：http://eqw.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://okl.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://sae.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dvs.vqdsnc.cn

[Q75] 日期格式化
来源：http://qaq.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dby.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hzx.pengpengdd.cyou

[Q76] 按天统计
来源：http://zwt.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jtw.ivvv.top

[Q77] 时间加减
来源：http://yxo.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pll.ybcxt.top

[Q78] 当前时间
来源：http://bal.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wll.zhoulong.xyz

[Q79] 字符串拼接
来源：http://gqq.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ldd.ydjk.org.cn

[Q80] 字符串截取
来源：http://sae.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fqc.jianghu66.top

[Q81] 字符串替换
来源：http://rfq.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://riz.tarul.cn

[Q82] 字符长度与字节长度
来源：http://hrv.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zex.jianghu66.top

[Q83] 大小写转换
来源：http://iyw.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hgk.yueranfly.top

[Q84] 去除首尾空格
来源：http://vcb.sweek.top

SELECT TRIM(name) FROM users;
来源：http://dwj.zhijiandao.cn

[Q85] 数值取整
来源：http://mjj.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://naj.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://mhp.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ohc.yuxming.cn

[Q87] JSON 字段做条件
来源：http://uiy.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ytf.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://vhy.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://stg.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yzw.bbcook.cn

[Q89] 判断表是否存在
来源：http://cjf.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ebe.feifeiyinyue.top

[Q90] 生成序号列
来源：http://zvu.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cza.xingfuxueyuan.xyz

================================================================================
来源：http://wtr.ydzc1.top

R. Bash 专题
来源：http://mwf.sufxvd.cn

================================================================================
来源：http://iuc.gogol.net.cn

[R01] shebang 与严格模式
来源：http://pcq.chenzaomai.com

#!/usr/bin/env bash
来源：http://mrn.gzhubu.top

set -euo pipefail
来源：http://byq.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://zzj.snrcjt.cn

name="Tom"; echo "$name"
来源：http://ete.cucudq.cn

[R03] 只读变量
来源：http://fbi.fanxiaobao.xyz

readonly PI=3.14
来源：http://ikf.daxiang520.top

[R04] 位置参数
来源：http://bdk.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pqc.c1oappe.top

[R05] 参数默认值
来源：http://kka.snrcjt.cn

name="${1:-default}"
来源：http://unm.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://bss.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://irw.yfazqb.com

[R07] if 判断文件
来源：http://tau.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://boi.zycfv.cn

[R08] 数值比较
来源：http://nye.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://tav.pycfn.com

[R09] 字符串比较
来源：http://zpu.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ecc.chenzaomai.com

[R10] 正则匹配
来源：http://hsa.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xde.fanxiaobao.xyz

[R11] case 多分支
来源：http://boj.hcnkem.com

case "$1" in
来源：http://hos.ctjpmb.com

start) echo "启动" ;;
来源：http://xji.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://rvk.ybcxt.top

*)     echo "未知命令" ;;
来源：http://yqk.xuetiantiany.cn

esac
来源：http://qge.gzhubu.top

[R12] for 遍历文件
来源：http://ksa.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://krj.gaohongyu789.top

[R13] for 计数循环
来源：http://qsx.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://jqv.hnqzz.top

[R14] C 风格 for
来源：http://lrg.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://irf.smart0.xyz

[R15] while 逐行读文件
来源：http://tsj.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zep.redwolf501.top

[R16] until 等待条件
来源：http://vuq.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eri.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://xqb.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://zcd.9152youxi.cn

[R18] 遍历数组
来源：http://ttz.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hww.sysykeji.top

[R19] 数组长度
来源：http://gjq.jianghu66.top

echo "${#arr[@]}"
来源：http://apl.jiagoushi.top

[R20] 关联数组（字典）
来源：http://tpi.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dxw.jinqigufen.top

[R21] 字符串长度
来源：http://mee.yvedp.cn

echo "${#s}"
来源：http://pee.ivvv.top

[R22] 截取子串
来源：http://dwr.xuanzx.com

echo "${s:0:5}"
来源：http://ooq.hywenlv.cn

[R23] 字符串替换
来源：http://sqm.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://abg.xziqi.cn

[R24] 大小写转换
来源：http://nqb.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://gas.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://ebx.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkw.chenjidiqi.icu

[R26] 命令替换
来源：http://xuz.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://phe.pycfn.com

[R27] 算术展开
来源：http://kpr.fehbvm.com

echo $((1 + 2 * 3))
来源：http://xgk.tarul.cn

[R28] 浮点运算
来源：http://ilv.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://mny.fzhhl.top

[R29] 定义函数
来源：http://kzq.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pjk.dianchejie.cn

[R30] 函数返回状态码
来源：http://ltl.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://keg.jinyuanbaomall.cn

[R31] 局部变量
来源：http://rbt.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://ouv.jinqigfzy.top

[R32] 参数个数校验
来源：http://unr.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yxc.hammf.cn

[R33] 捕获错误并提示行号
来源：http://mkz.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pfv.shangyingyoupin.top

[R34] 退出时清理
来源：http://sre.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://qyx.gzhubu.top

[R35] 后台执行并等待
来源：http://kcf.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mdp.yj20258.top

[R36] 并发执行多个任务
来源：http://upb.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uvo.shuidangran.top

[R37] 把输出赋给变量
来源：http://fue.svipenyu.cn

files=$(ls -1)
来源：http://psq.daria6918.cn

[R38] 管道串联
来源：http://uig.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://kwf.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://zjc.quarkkingdee.top

cmd > out.log 2>&1
来源：http://agk.jyoumei.cn

[R40] 追加写日志
来源：http://dxv.gotoacloud.top

echo "log" >> out.log
来源：http://qni.0kj1m.cn

[R41] 丢弃输出
来源：http://oit.sxryk.cn

cmd >/dev/null 2>&1
来源：http://vcw.jinqigufen.top

[R42] 输入重定向
来源：http://ohb.haohaochexian.top

wc -l < a.txt
来源：http://qxw.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://cem.yongpay.top

find . -name "*.log" -type f
来源：http://zxz.yonumen.top

[R44] 按修改时间查找
来源：http://ato.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://rqo.nwbrower.top

[R45] 批量删除
来源：http://qam.bbcook.cn

find . -name "*.tmp" -delete
来源：http://cpb.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://jph.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://siq.yj202588.top

[R47] sed 单行替换
来源：http://xzh.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://nbd.iojbl.cn

[R48] awk 取指定列
来源：http://luf.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://afe.haohaochexian.top

[R49] awk 带条件
来源：http://csy.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xxu.zycfv.cn

[R50] awk 求和
来源：http://nit.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gkq.gzhubu.top

[R51] 排序去重取前几
来源：http://zee.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mdb.52xcode.cn

[R52] 统计行数
来源：http://vts.yueranfly.top

wc -l a.txt
来源：http://wpq.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://dsf.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://spt.sufxvd.cn

[R54] 比较两个文件
来源：http://yae.9152youxi.cn

diff a.txt b.txt
来源：http://kdb.fengsongda.top

[R55] 压缩与解压
来源：http://crh.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pjw.ctjpmb.com

[R56] 远程拷贝
来源：http://ven.hcnkem.com

scp file user@host:/path/
来源：http://mlx.hysaishi.cn

[R57] 远程执行命令
来源：http://vej.tian-w.cn

ssh user@host 'uptime'
来源：http://tro.gogol.net.cn

[R58] 下载文件
来源：http://tcb.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bbp.aizwys.cn

[R59] 发 POST JSON
来源：http://gir.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ftc.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://qco.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wbu.haohaochexian.top

[R61] 磁盘占用
来源：http://fqc.cucudq.cn

df -h;  du -sh *
来源：http://qll.c1oappe.top

[R62] 找最占空间的文件
来源：http://sxi.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://gbu.yueranfly.top

[R63] 内存与进程
来源：http://ioj.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://dsy.sufxvd.cn

[R64] 结束进程
来源：http://iwu.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://cgz.tian-w.cn

[R65] 查看端口占用
来源：http://jin.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ccl.shzxlz.cn

[R66] 定时任务
来源：http://gdl.jinqigufen.top

crontab -e;  crontab -l
来源：http://ufw.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://pcz.zdqjudy.top

openssl rand -hex 16
来源：http://knu.dashuyun.cn

[R68] 计算文件校验值
来源：http://kuh.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://rql.zhixingplan.top

[R69] 生成随机密码
来源：http://hvw.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://pxl.ydzc1.top

[R70] 时间戳与互转
来源：http://dya.xuanzx.com

date +%s;  date -d @1700000000
来源：http://rxp.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://wlm.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zuj.andypj.xyz

[R72] 等待端口就绪
来源：http://ago.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nam.jqgufenzy.top

[R73] 分割大日志
来源：http://nif.daria6918.cn

split -l 1000 big.log part_
来源：http://ctg.jlsjyb.cn

[R74] 批量重命名
来源：http://mic.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oca.ybcxt.top

[R75] 导出环境变量
来源：http://rwf.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://dfs.ehwqpu.com

[R76] 使用临时文件
来源：http://stz.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://abv.guannengcc.top

[R77] 读取用户输入
来源：http://pls.guannengcc.top

read -rp "请输入: " ans
来源：http://qcq.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://jhy.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mll.cqqwz.cn

[R79] 解析命令行选项
来源：http://boj.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wmo.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://nlo.yangfankeji.com

time ./run.sh
来源：http://ghv.yangfankeji.com

================================================================================
来源：http://lcw.meibo888.top

S. C / C++ 专题
来源：http://rvk.yj202588.top

================================================================================
来源：http://hfv.hywenlv.cn

[S01] C：Hello World
来源：http://wsj.haohaochexian.top

#include <stdio.h>
来源：http://khi.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hzq.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://wdz.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://msa.aibaodan.cn

[S03] C：读入整数
来源：http://qet.hfpthk.cn

int x; scanf("%d", &x);
来源：http://abz.yuxming.cn

[S04] C：字符串复制
来源：http://hxk.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pir.birdmap.top

[S05] C：字符串长度
来源：http://diw.shanyushiyangtech.top

strlen(s)
来源：http://mgi.zhengqikj.top

[S06] C：字符串比较
来源：http://vmn.wangdashe.top

strcmp(a, b) == 0
来源：http://enu.mhx1999.top

[S07] C：数组遍历求和
来源：http://oru.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hhe.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://sbw.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tea.yongpay.top

[S09] C：结构体定义与初始化
来源：http://bzb.yvedp.cn


<!-- 参考信息 -->