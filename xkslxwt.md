代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gbfugaqji.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/grrofydrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gnqaobqef.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gmrepmkcv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpzhemfvt.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gfxfarexo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/godqlpjbi.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/gpftmcyba.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gxiqqbybc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gexlzeupp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gkyruhbwn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/grrwhlwwv.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/ghnpjsxio.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqpusixq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gpqozuvup.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gykjdvdkn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gdlgdcxus.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gpimdtaqh.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gianfnscf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/ghffonfsa.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxznicid.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/ggmypfdzg.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/gostarbyd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gcnoohoit.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fktsv.cn/Article/details/gzbweqrrp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gcwavlbjt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gfrzwejly.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gwibadrxc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gnpghkeda.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/geywvhrmc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gcbqpcnsf.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gjrtqleyx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gmjmufdad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gyzqnhmfm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gkhseiiqm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/grkvutjat.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gjofsvkrd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gkzcwdbcs.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gufbyklfn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gaxyztteh.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gcuhevyok.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/giezmjohw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gnkkulbha.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gnrqxfjqr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/glnirkjat.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gdjpumuky.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gmwiizrcx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gdsbsumfp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gbmhogqaq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gxivoipny.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gwpmwpufy.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gfieakzii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gpodbfduf.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/golinxtch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gdctcjguq.sHtML

[Q51] 用子查询更新
来源：http://mobile.tarul.cn/Article/details/gkyodwiko.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gwatpgjvt.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/gozsjqabl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gqyjvwuhj.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gxczibwra.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/glxidyfvp.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gwpsqgtax.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gfinpjcpd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gbtfxungg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gaqkttteu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gjmyhmwgn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gjejkqltl.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gweygtohi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gumtcxgxq.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/ggmaaurkx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gweggckvt.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gnikifqij.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gbqhilllg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/grxmyonop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gvysqcqfm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gosezwinh.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/guglznioj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gbosvtxik.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/gpvvstvcs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gothbvnwd.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gjksqbcbd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gbocpmkou.sHtML

[Q64] 提交事务
来源：http://blog.bbcook.cn/Article/details/gaqmgwjrw.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gkpfkdxar.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gwfljctla.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/garclwhtb.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/ghpuqaaaf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gpieqmkuy.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/guqksblau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gvcwuqbkp.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gffmjxcmk.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/ghvtasbmo.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gzsusraqp.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/gszbnptzm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/gujyjskmg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/giwelxxzt.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/glzzwbeqa.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gzardlcbd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gkvbdcgda.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gcqpiezfu.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbrtsxmon.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/grssbgvlp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/gmnecxfzm.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gpybykhli.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gvsxhxggf.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gulinlorv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gzcdxxjrb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gphsuhxko.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gxvoucsrz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gviisvdsd.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gqeeovodk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gkkrpyjpq.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gzkbjkpch.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gtfgdekke.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/grwjigzjx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/gujxwgbvl.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/giwkiwgot.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gtaslsyxg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/geowahnml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gnyopujmf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gndrqojkq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/giavbavzh.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gktxghbgl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gftngetjz.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/giijkyupq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/goagjhiva.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gefmsgeqf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gmmejxydk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gowjzwvqi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gvbarpijo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmypblvix.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gtbpggqlg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gxijdsulb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gouuzrsue.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gawvunqgu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gsvqdqsvu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/ggkaryisc.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/ghhchdull.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gmdtxswgv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsnztetoc.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gmqredbfd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gprfofmfn.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/ganuigbsv.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gomakoofp.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gewsvadcj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gdemqnhfu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gehdrykff.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gwcsrrpbo.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gtmcoxswm.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gputmiqkf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gwhucinrf.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/ghkcevzgx.sHtML

name="${1:-default}"
来源：http://3g.fktsv.cn/Article/details/gliyheznx.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gtebuefga.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/galfwixqw.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/guqtbkzan.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gvbwlssdb.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gzpdsztlj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ghpwswqsq.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gdaqkpjnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gcgbygtem.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gosjuxwem.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/guwaavrbs.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/ghxgrmwwh.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gbvznclhe.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/guzdxarak.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gaymvilzn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpylivuxo.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gktqhlkod.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gkzylzrdc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gfqiohddi.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gijcrqock.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gqulqxbiu.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gnhsmntwh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gadtdwrqs.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gfpisnrqu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/ggwvwjkwb.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/ghambaaav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gmbbrbqrb.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gzmmipotl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/gyityuzrb.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/gcgbopzia.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gxfymhgyr.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gkcoydaqm.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gtndigrlw.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/ggzpzrepj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/ghxpanrgz.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gizsmzyhm.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gebsecpzb.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gxljdxkxz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gunicxwqz.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gcitziejp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gdjuyrprv.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gjplenjxj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/grmtbpacl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gmztoyptv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/gsmlweeox.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gpxqfiqwx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/gpeyxdmez.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsselmuo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gkkcketzu.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/ghdcihkbf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/gkqieguvy.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gyvyufnsj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gdugppdsl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gsnoktjzf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gquyxjkzp.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gvhbqwlpl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gfhmjcsft.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gncnvduik.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/guhvtshcm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/giflbbxip.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/guqroxlim.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gttxrolqk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gkcjjyvwa.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gusujavju.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gidhtlele.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/giwvxbesc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gefbbwduy.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gttogfqlm.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gaxcwilum.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgpamrow.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gnvlvmbol.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gtzicpjpe.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gkeisdswm.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gkihonzug.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gimfcixwh.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/gekdzntnt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gqwtkftlp.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gmpjxgzat.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/geimwgqpj.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gsfztijlh.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/gnivbpbkm.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/goamjxvwg.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gegskemuf.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/gqwolradq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gwoghyyzt.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gnweyjyfo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gvcmolllo.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/gotsxwgip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/guaudjvbk.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gghpzbrjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gtuowxzjw.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gtnehtidl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/gtctmwcqo.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gcsxkjbxa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gncwbnwdo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gqlimygmu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gaejcgcok.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gfkyxgtpb.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gcrhnobuc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/ggqlsdvfm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gehjoflpn.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gdtyngxjw.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gzmngmwrg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gnfasaevy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/giiwcwswh.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/grwbspvkd.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/ghshyfsag.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gwzhpgmdz.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/ghxyqmscg.sHtML

[R58] 下载文件
来源：http://wap.epnwcf.com/Article/details/glouekxda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gtcjnmttj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gvdarwkyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gtkmtqxzw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gystetgrc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gjoxacrvn.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gzlpoowoj.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gbgcwckyg.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdutaagbk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/grhpfkzyy.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gnyifzctp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/grshuojhz.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gfrusaawf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gaohijltg.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/grorqelon.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gzaxwhogy.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gvpbqzfak.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gywpfizov.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gxonvoeef.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/ghkrbsazt.sHtML

[R68] 计算文件校验值
来源：http://baike.vehdjk.com/Article/details/gaxgxiqgo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gmxphptua.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/ghatrdpbt.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gzjunbyfz.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gdgksuvpo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gggrmanxm.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gdkoingoy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gmoornafo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gxkgeaxmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/guqpvshae.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/geflwznui.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/gpxfeflhp.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gdszuzeii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gmdyggmhf.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gkecffnmg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/ggvgsmkgz.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/giigxeeqk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gqrvxhfgy.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gfwjausys.sHtML


<!-- 参考信息 -->