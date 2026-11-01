代发 wailian999

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gkbiivqjz.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gbxhjskve.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvylrmykp.sHtML

[Q17] 条件查询
来源：http://m.share.tarul.cn/Article/details/gonnqqxoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.epnwcf.com/Article/details/gsenyqidt.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/giegzmynd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gdpvlkreb.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gqrpnsobe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gxbpeuvqv.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gskpuxxlz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/ghndgtqyn.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gpxkqrmtd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/guxnxzcan.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gzlkbxvuf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/grpzwxzal.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gfpijubpg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gdypmpjsw.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/ghxwwsmkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gjkwrheze.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gyiftsxdq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/geyipfeum.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gcqedvmhk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnngafsef.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gkagidcwz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grzamscgm.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gwbjpnmyc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gbgrfeajb.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/glhhpipye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gxtlqdhok.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gfzeylzqd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gjgmxbutv.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/ghfkftswv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gfwkqxabr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gxyscehxj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gnfdqiuzi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.tarul.cn/Article/details/gtdfqkder.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gqopfrhaf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gwjbgjdrd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gbfkwgplw.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gdaalapnv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gjivpgbwo.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gormvfxmp.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gxbombrpj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/glbkkvhou.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/ghjycbrfn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gukknhkku.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gttbjbmos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gnjcmczct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gishlybne.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/ghrywkcms.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gqjkxnwuz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gfeplcwqf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gtxmrdirq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gpsjjorkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/gilpsphkj.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gwgbsztqm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/gqgagfmxz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gxwckgfim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/giwwgjzqd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gssozntia.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gsqasrnwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/grcxvjcme.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gikqpiqtq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gjfeijhan.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gzkaddqpy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gvwsznvyq.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gwatzlawn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gnjdegzut.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gzfzxuihw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gdwzxudkd.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gswmkbnpj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/ggbymagzb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gruakqumb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gykhunmkn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gpuapuwzr.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gducisaai.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gcrmpixsq.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gtcolwpui.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gurtvhgwp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/guwyuxeus.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gsfddvmwq.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/guvzxpxce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gabktnaah.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gyxkckqfs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gplzxflll.sHtML

[Q54] 清空表
来源：http://mobile.bbcook.cn/Article/details/gnwmghcwh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gbcnxlapx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gkynrmpww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gkynuxggq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gpgabjibz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gpencacbc.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gxcgwfabi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guwwqklru.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gnjfplizi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxlzuyvo.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gejoubwdy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gzqiiaieb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.vehdjk.com/Article/details/gkgeoxfdc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gdqdqhxff.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/geullmlae.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gqfgrcbsw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gzqcfiuwg.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gnoknexcf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gxkeoidmu.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gjzhpspwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gnewtkmtw.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gblkbgpvx.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gilynjmlc.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gqnzosopu.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/gbcokqkhl.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gwdgyjngy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gbvypffgq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gsrnmwsby.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gxblbwveb.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/guwerrafe.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/guksponjw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/ggrgdenal.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gnyznikqf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gpmijncyg.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gidsakcrr.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gtkkbwcjv.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/gxljmeqdm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gnqwmxciq.sHtML

[Q72] 查看索引
来源：http://www.share.vehdjk.com/Article/details/gimthrwon.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/ggepmtixp.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gokxnxbmc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gluedjgaj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gmrgyhnex.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gcyjzvzrh.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gqijuhiwo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/ghexclhvd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/godypahde.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gvtbxajuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gcmmshfqq.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gshsvoymz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gofukvlvn.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/giecnoplc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gwzylonhp.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gcaanvgau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.bbcook.cn/Article/details/gnjxksglp.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/gtrhhwjgc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmzumjbrm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gjmgtdkbl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gpyrucbgn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.vehdjk.com/Article/details/gldjgffke.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkoyqojlb.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gaphmsbfr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtzhijifc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gcpsmisge.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gfzjqisuw.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gxfiginka.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gzbbnnogs.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fktsv.cn/Article/details/gnwexdeqn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/guseohdes.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gogcivkpt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gqdanqbei.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/gqcuvtuqa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gqxohjosl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxkvdxjfo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gumbbuczu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gvscbeljc.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/gszneotmb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gxjuydvqn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/geyyhjinj.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gjtxbwlcv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrzzehoj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.yfazqb.com/Article/details/grcpyvtzw.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/gkkptjuer.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gjsvzjakz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gjctixfju.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gqendehwj.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gxichipwz.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gtlvdvude.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gzbefmurk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gqscssapn.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/gpfdpdtjr.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gjkzsvdrl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/ghluqautk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gxqikzqel.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/grepaxbzv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gxbwgihpq.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gfpyqdsxu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gunjuyoxp.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gitfxijyo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gqmjsvwia.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gijcpugpx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gpggilivr.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gkxvhqiyl.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/guaqrxmsb.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gymuphglb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gescmjkxp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gwylxmkxf.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gdkneqtbu.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gbxiyifsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gnrlkohjn.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gfqvsxqzu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gifkqeauf.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gjwylrcte.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gfbpwxwir.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gslphylus.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/ggsgmjtqt.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gnukutqyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/guxnwmsmr.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gafapgqka.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gqcrgdkyw.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gzlmcexer.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gauwkzmzu.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gtfuiifuv.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gppmffmci.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gmdobujmz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gkhnzzncy.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gylqyvbfy.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/ggopkydhm.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gdqfrwkil.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gfcaeiuow.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gfahbzoej.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gqdbtlhml.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gpscyljha.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gvskqikvk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gqomgofch.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.bbcook.cn/Article/details/gjlrtrmzj.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gzimjnjif.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gkzkobxux.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gjpvsmgsu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gjafbmddr.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gimpwcmmu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gfjlasvul.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/geggdetpm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gyjvllcjf.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gtkbltyry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/grluuhtak.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/glferquez.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqpqxbhnv.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gtrzizlbp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gdzacbtfi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gcxusmupj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/guyslioau.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gddqqhraz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/ggsvmsuow.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/gpaxkmnpn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gvjzyonzm.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gixbyqldd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/goztqpkvk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gvhtaiuav.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/grigylgeo.sHtML

[R38] 管道串联
来源：http://www.m.share.tarul.cn/Article/details/gghtkjvut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gwiqhsfpf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gblbxtqop.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gthswgrcr.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gevbehbdm.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gwyetrjqq.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/grfqqxbeb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gqhtcxegv.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gdopxammu.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/guevwhqxs.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/giqirtcmn.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/ggbbvzeow.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/glmvfvmbr.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gegcnpsih.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gfwdtqgza.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gowzaqbae.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gntddvfzt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/glcadlfog.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gksqtwdcd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gqqkiwdfg.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/glrbvwmig.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gwiojfvpb.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gfozymjxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gvmrutygm.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/goeewesjl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gkxnvfejt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjafnslz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gczevloej.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gawemedop.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gpmndvodv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/grfpvgiwc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gkobsvbec.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gdnmrwtyl.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/goyjclurs.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gvfnmcgei.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gjodegwar.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gfcvtuxdj.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gzqfqctmv.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/gmiagiavy.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gcdausdbs.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gawuqhcqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gyivvjgqq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gdctwdpic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/goumsosbz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gwwjioedd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gsutiklzp.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/ghszehygi.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gnbbbfmre.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gpvwevmlj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyyvzeww.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/ghioxrqkr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gotfirnds.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/gugituwel.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gfeuasfry.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gzsnailiy.sHtML


<!-- 参考信息 -->