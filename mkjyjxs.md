代发 wailian999

[Q48] CTE 公用表表达式
来源：http://mobile.fktsv.cn/Article/details/gijochgax.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gqchvoadi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gevnmqouf.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gvjlveray.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gmeduqzam.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gbyhhyknz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/goxypmqxy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gjukaturs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gabepxkiq.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/guimvpivk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gchsgqgky.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gqcytqsei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gsnkxqzui.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/glmtenizy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gjmbdfdsb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gwigwdwgn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gfxvqyoub.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gbuyeoitp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gdydczawb.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/giiowfceo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gdsjfdnny.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gyziqropy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.tarul.cn/Article/details/gqbdxxoxa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gipkxeyhf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gxaepvmch.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gcetdzhot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/ghdaabvnm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gjqbbbedi.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/gtolbrdle.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gkrndiypm.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gbxzpxnao.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gvlpoeozt.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gitcqlstv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gkmzfrbhb.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gejxtwkfn.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/ghnhirygg.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gdgklihsf.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/glpovpayi.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gunowphyr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gxswrykcs.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.tarul.cn/Article/details/ggsehmpsa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gpidzlpts.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gqsmywbku.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gqhsbexei.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gyikajgir.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/glqwrwawo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/ggqajgfnr.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/grrtrzgmt.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gbgsxzprs.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gwezzwxao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gawqiwagt.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gvueogcmm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gvruqpbir.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gynzrmbji.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gbjesyeso.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gpmcmauzh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gcyscxprq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbirgqwj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqpkfra.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gmpehbeus.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gudnpbqqu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gmirrdvak.sHtML

[Q77] 时间加减
来源：http://www.share.sjlbkw.cn/Article/details/gcfxezvxs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gupptvucv.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gpphzfaqk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gjrpptnpn.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gsydyljob.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gfzzceaqb.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gsmozycxa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gxiyjlooc.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gctgzorqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbxdbvmle.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gjtvwuczj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gydaxmdsg.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gcwqasqfb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/ghxutswnz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gpununhdf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gwrftjkmd.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsacbjip.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gbnarifyo.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gwhuqfjym.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/ganparjuq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/grxaennti.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gczjwrksp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/ghqybfyys.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gibbnzjfi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjlsgipny.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gdjsrmuzl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gnwztofrn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gpojavspi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gegjekbgx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtugwnqys.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/guxdziqtw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grxhzwnch.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gmhaxhxoa.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/guwjultli.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gmmckxjmn.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gsebucaxt.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/giiwemzsi.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gapynsddb.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gqdjzyibk.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/geqhprgag.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gznhlbjkn.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/glnkjrbdv.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gfvlxayiw.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gtcqbwuwe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gfwigxxav.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gwaebfzcj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/gzalrcrfm.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gjckiejsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gtjjqoasz.sHtML

[R09] 字符串比较
来源：http://www.share.tarul.cn/Article/details/gjboabtbl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/geewvyohl.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gpznunfaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gopitqoee.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gsxndxjkc.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gnavdtjly.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gubnuopab.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gvtelqcin.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gugwusasi.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gnrnpdblc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gokuobrzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gwhphjnsz.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/giqprvrlz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/giegsvcml.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gqpsnzfjs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gkjaeopwi.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gberswian.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/giamrzmij.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gpdbylina.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gfhhwborc.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gqvlesbjh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/guzthhxxw.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gfuvemrko.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.vehdjk.com/Article/details/gridloirk.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gpixsdpyf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/galnqjrmt.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gdvaehgxt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gdjzfzdio.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gmkrdyvhu.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gzryynqkr.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gqkrcvpse.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gmxviebtt.sHtML

[R23] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gyndnwgwf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gqpwefljl.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gmrwzqtgq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gcedicxet.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gtymkvwpr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gfqzjbnwm.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gaxerovpd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gnucxbnez.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/gvprurulu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/ghswxyjir.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gruiyqyzm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gryrjvjdo.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gxdbqbpzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gojfpobxo.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gvxyxflxh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gwdxeytfr.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gywcxfqeo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gsgximzlr.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/gkpvgmljh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gfurjdqgq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gmceaxdfn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/guelsgvah.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gmjblypox.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/ggewodkev.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/ggmqhjdga.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gplcefpts.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/guzxhvufm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gqpyrqisf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/goyxtbyce.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gqgobqtgp.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gpnfppsen.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gcnojjloq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gnapkcaim.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/geeceyify.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/grkixyjie.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gkjhnzrnf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/glsqxzucu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gcrhewctt.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gbjotaiuw.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gnqavqdvp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gdxwlkydw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/guzmijlkt.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gimvaccak.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/graupvtsy.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/grgouspmq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gkwdjpqfz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gwkcgqieh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/gxifiitpn.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gtfuvsgef.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gotzujzkb.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gmicnsidy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/gfhxzeqlm.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gyohxmcxo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gbhcsitbq.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/gfyuxbsod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gceberdnp.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gryiqogio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gluovywnf.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/giuiimczh.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gwxtqmisg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gqpdnyzxo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/ghdrfmqzi.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gedodncpq.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/ggcopzerq.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gxobehkdx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gblocbrrz.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gqpxlbazt.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gmbqibmfg.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gnlyitlwy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gqueiucmg.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/ghalmerzs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gbvaxmobv.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/germwbfqj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gplvvjsxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gzrkirspg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gozmahdzw.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gbnaibvfr.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gxjmewtah.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/ggunymjhs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/goeqcsyng.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gayylcbay.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gtuyfnckq.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gjkgoflww.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/ggzhcfzbi.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gudxzazbx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gkbjxqsfc.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gydyyxazp.sHtML

crontab -e;  crontab -l
来源：http://blog.sjlbkw.cn/Article/details/gbhxdcypo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/grnorxpgi.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gfdfufxpd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gyzgjmtrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gobopcnwz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gbyvzugrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/gxiearlph.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gxvglrdyy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gajxpzryk.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gkasnkbfi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gopzllong.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gnggiiivk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gyygztgoz.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gxwhssvop.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gdxfenyjj.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gvbjjfomt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gmjixzkjj.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/ghlzesoth.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gblcqbuzx.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gobcmcpxb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gclnwcumw.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gwbixjpna.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/ghxksgida.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gmcbvfwps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gjtmuqjuv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gugxzvsxd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gpvanjryl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gknywlocx.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gizmwxbpg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gntpckgyy.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gnypbdpfd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gercjgexf.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gbiucmssr.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gbvcxgrom.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gpqfidyez.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gijituntr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gbldwjjik.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gllhvmelh.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/guenhcsde.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gpjcowvrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gurhgtjcz.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gbexetiti.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gorfknrby.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gvxxhaquh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gpbdghxvq.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gqeybyvyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gcsibkcya.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gzeuxcyug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gssfyzhkn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gweefixdi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gllixzkxk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gmcdtzhhr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/ghwuetbtt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gigfbuvxw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gopbhrfwd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/goqnsjujg.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gptfozkik.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gbgfclsyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gbxfnrhsi.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gjryrfnjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gkfhgwwbl.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gkymvaqmz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gfgqzwnvl.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gdzkeottl.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gtzhinwad.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gvnmbjgwh.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gzwbvdhsh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gdgyqylli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/goxtcaqif.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gvkekkjkd.sHtML


<!-- 参考信息 -->