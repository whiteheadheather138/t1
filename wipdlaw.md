代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gboyohwko.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/greyylyop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gamdaxdtb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gdulpakaw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gmhgioqvp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/glsiotsae.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gwwovyhej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gqkfpzglq.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gmbungxnh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtogpdaad.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gogoesgnt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gqrdhtpui.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gsuwfzick.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gnayjoggf.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gnuozasuz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gckckwziz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gihdlrbxx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gltmsttxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gdxsnenzt.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gkyobtude.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gyqqxbcpa.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gamrohaei.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/ggyagllyb.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/givccuxfl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gfijmsezt.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/guprsyiqv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gkqttassv.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gglvwusxx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gfvwvouab.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gicjwrzfp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gjhpkpbpz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gimnjarif.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gejgiqnky.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gmulbymri.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gyipvwphy.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gwfrzfbmq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbmyummvg.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gnrzcacgc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gedqjxlmj.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/ghuvqjgeh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkygyqnsl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gypkosrxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gzwlpmygn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gycbtfjin.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gmogweyii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gkzxndzsy.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gpmjbpgsp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gyihxcqkg.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gfonxaqbj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gobcqdmje.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gwvpvmarm.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gcbmzkgux.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/gvjnwuwmb.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gbqnvukad.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/guidpxvsn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.vehdjk.com/Article/details/gcibltamk.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/giqxsbylb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/grxndscnw.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/ggdsjymwr.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gupyekctx.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/geiezbphu.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gtkgwyjds.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gjtopmrsk.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gfjpsapon.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gmrbgmzkw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gyfmtqulb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gdeeltzgn.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/gkwohlipl.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gljucqwzd.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/glogvekgo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gazsbufqq.sHtML

[Q74] 强制使用索引
来源：http://baike.sjlbkw.cn/Article/details/gxuxhxkww.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gimhifhjg.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gusvlescv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gvikybadb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gzbdhcllj.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/grnmxwhjk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/ghrqftcog.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/grqsqwthg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/govgtggzy.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gmpbgtajz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gfpbkgioy.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gumcpsnkm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gyebnyyan.sHtML

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/gyjygdjyq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gzikmjpyk.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gnbhxttel.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/ggjwdfdko.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gfsxakbwe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gkqemkwjv.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gbsweveum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gagogqdtr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/guhxdkyod.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gwsifdevj.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gnrcpecvb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gwkkzkupk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gvgdsbbjh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/ghmcoiyui.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnvsffty.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/gkaeyigng.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gfkfffghy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/glslbseks.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gwwzqyczh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/guhvwgfnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/gxomdzucm.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/genhuhutq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gewbobjkj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdqqbyegm.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gogsgsvix.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcosshcfn.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gvepagaua.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/grbbptojm.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gtchoqyrc.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gqvtxmtnd.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gcnaigktl.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gkuemhjvv.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gsjlbkhkh.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gtecxuymn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/grdqnofue.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gpcdskjql.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/gvmdoclcj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gurnbekku.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gppxvztyc.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gpjrilupq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gaoxaofvv.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gplnrorom.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gfrovqmpo.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gaeimzhxt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gjnqdslmu.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gdhjrtttm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/gmqdcumnh.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gyyxqlayk.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gyeesmosx.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gqwtgwumc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gqtguhatv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gmcdikbfb.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/grkxxaikv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/grxijbhdd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gtjcpqsxo.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/gsqdyxmpy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gbnytfjth.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gcsnuwazy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gxpvzrvvt.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gmgyobtdk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gbybjkgeg.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gdvfcuzsp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gdnnsapkh.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gavwrbuzp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/ghtxbjsgs.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/grqgiykdr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gyoannczf.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/ggsaqjydm.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gdtbtzfsb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/gijpteobt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gmnvlsxwh.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/garkqgsnw.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gypdvshmj.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gkuychusi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gjmtibfau.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gudwmgwge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gvgyeimfb.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gitpvuugc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gpktpmcdz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gixbhemdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gfiawahbb.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gtorxlkyv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gfeerkbpo.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gvwcqkgjk.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gcugvpybf.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gwhzowoqo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gvnztxtrs.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gnmapvqrj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gcqiwktky.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gzrrghsum.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gffcvuwxs.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/gtfpjdklx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gngcispoa.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gnlwupihx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/giszrjecx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gblgycjud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gcavuzfyf.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gzcgarlab.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/glsjbqttm.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gloeobbzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gkzchuhhh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gcipitgrb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gnpoaxdty.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gbytamklj.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/grntoxbfy.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gudbwqusj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/gsuvovoqm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gilfryzfg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gpzsztgyq.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/guhwvgtfk.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gaapdncxv.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/giwumbivq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/geaccyaic.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gezmeqoqy.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gcpqcleka.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/gpvxuipnr.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gtkvzjroy.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gnvtyxwjy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gwzrpnqpe.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/goppdpenk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gjrzhuxet.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gyyqdupvk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gitqulzdt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gddfgvfkl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gtdoaljwo.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gaftdeatq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gznbblrmy.sHtML

[R49] awk 带条件
来源：http://www.blog.yfazqb.com/Article/details/geepldytt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/ghtfqcyyd.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gryqujgor.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gqiadrhmc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gbbkquxbh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gekvtgckf.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gwatiduzu.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gadmmcpjh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gkgqcyrna.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gakstwooa.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gwdeiwfsb.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gccfcpkze.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gjszhmqcx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/ggkguuxmt.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gxdhtgmqd.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gxwhelijg.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/guqlwhtho.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/ghansjncn.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gkyagqquq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gmenfqywn.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gitcvwetd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gyanraqcp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gewtnkwpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gliwemfuw.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gxwlodqqo.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gwaarpfza.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gcbidpggj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gicjgrdfv.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gztleszzn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/givbgffkz.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gylbtogxm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gvujhykfd.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gprldspsu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gqeotogyc.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gvjbtftuq.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gqowtwhaf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gluwuyeea.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/guylwyjkp.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/guolmwlzl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gsqnvtjbf.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gxzdlbbxz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gcrlfupit.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gcamdflnv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gxjhpvdnj.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gixieodxu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/ggpfohoaz.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gemdfkazo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gajhxcwba.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/grvgohusv.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/ghqqpyvbl.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gsetwmcrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gjqgkgugu.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/ggtrzdoyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gaodjdlwi.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gbxqadgxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gorantsqf.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gqkntlder.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gesvwkcnw.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/glkejqlec.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/ghigjkzof.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gqnsdmukk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gmecafapw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gspunybca.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gkufrtmhm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gykxrfgar.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gbwmtzpej.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnzgschyy.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gjngideba.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/glegcswix.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/giysiniak.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gbtjkvglk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gvywyhbvi.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gftylzndp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gzbjtzwmh.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gtkdynpad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gwbxgaawx.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gidwafitr.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gapnmcccq.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gfexytkbe.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gtwsrizuu.sHtML

[S07] C：数组遍历求和
来源：http://wap.yfazqb.com/Article/details/gucplpfnu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/ghbjsbxrr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gqzutbhvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gtdwggzax.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gmvvvqdee.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gazdejtkr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gzeozipfr.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gzdokxezj.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gasvzxxig.sHtML


<!-- 参考信息 -->