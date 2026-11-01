代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gcenhqpqs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gwtysjpft.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/glrlolofk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gfjkomuso.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/givwwbjjl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gpuhxhgle.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gwlhcukjw.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gpviimttk.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gxzibpohw.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gumtvkuvf.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/glxhuimxc.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gndjdduau.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/ghaupmqty.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/geyywudnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gpptodysd.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gzwerldyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gbbvruppd.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/guxqcdzyp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gmmqihsna.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gttvgafge.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gjasrjqob.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gbpzfcagx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/ggevytosg.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gcyrrenwp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gaxulpxwp.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gvszvidde.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gkmqzuung.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gpohoedpx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gmealriju.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/gyghxqtry.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/ghqhmkysz.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/ghtpxqwnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gvvjohyok.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gekkvsigy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/grwoalzmm.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gvwiicshl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gyzulmxfc.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gfhcxetjk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gwjvrwmpw.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gahgfffqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/goukpboxp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gebiocezc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gjwlpftax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gtforovrf.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gqqejvfpe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gqmweqvin.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gcinwrcnr.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/grmvslefe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gdlzbafpz.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gajqfzdst.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/gbznxmsza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gwdiylqts.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/guwvmahzp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gwwdpgdts.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gnijsuudu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gfkujmcju.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gadgoniee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gguzrjdwy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gzuktmxgo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gjqvcjrrd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gcawjevcu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfogqtygx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/glwappzrl.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/gpgbamukn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gjqhesxwz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gptnnbgtd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gcnjmvagx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/grubcarkv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gswtdvdtj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.bbcook.cn/Article/details/gjzlhxjqp.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gzltuwtdw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gqbzdluxc.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gjenshcxx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gcxqugmli.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/giwcmyggz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gxthmjmxe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gpyysyiou.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gdnkndeoh.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gcdlibbhy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gqmbkckbo.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/gprohopab.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/ghvnqwega.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gilxmaqvy.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/ghrmtwpnv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gqypggqul.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gubirqcdo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gjmfvebia.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gnixrxjvy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gxaszmbxj.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gobgiddrb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gwzyjorkb.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gajaahoov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gokrvwpxr.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gzaufyxvh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/ghkgmvksi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/gqkxsvyct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/gwenkzmmd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gqyeqcgpy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/goovuqqaw.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gcmkpephn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gkyioimxr.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/glotfacdw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gsmoxxopn.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gaktcwvlb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gchvlgqsi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gmfnzdotf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gbnueszfa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gblsncwln.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/guaiftzqz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gsuidfgzb.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gemxfxdfg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gfrzvypul.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/ggjhksihz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gtiquwimp.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gkmffepwd.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/guhagresn.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/gxgbqmymk.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gxrpbngww.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gwhjzcvti.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gbhrrkrki.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gysshlqgl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gljwcpvlg.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gpykfyqam.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gfnijnqlu.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gliaqdpyc.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/glzxabwvc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gslewtled.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gralpzvtc.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/ghnitaeby.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gsasutrrz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gxejfbgus.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gwqcgujin.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gekeddfwf.sHtML

[Q73] 查看表状态
来源：http://www.blog.fktsv.cn/Article/details/gcokhjzus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gjtnyzxzi.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gnzejolzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gwmuffzkw.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gdaifasvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gmjzilnxv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gabzeoosj.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gowqdbeji.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gbjhkphnx.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gvyezaobj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/ghmmetxfo.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gnzutdlcs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/grpvmznpo.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gxdfrnbgw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gzhxkzsry.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/godzksvwj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/goqlpmwld.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/ghrlrmnwd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gfebzdvwd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gngqmvyot.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gctpkmvnl.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/ggkvkfget.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gfonlifhf.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gyledaflc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/ghseqqqjk.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/ggcondqtw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gfngurcjj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gwepxdexn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gfsskpfhs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/geyhosxth.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gjgrqdchs.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gzznwvxlm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/grumnvxuo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gzjeokhti.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gaqjcbitn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gwvpwhsjg.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gfesqclxk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gbrzexjqs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfvzlrwdy.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gaulrvtxm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnbgkmdml.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gsbcjartk.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/ghbqjnhln.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gxfsfrgot.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gnngmvlva.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gefijaxie.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gksylgcdz.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/grxbxmvhy.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/glkyhkazs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/guleaszxq.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/guonyfplv.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gmviwxiez.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gphwvdtyd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gcvfbqsfv.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gkktvmtkf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gidledncc.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gmtpufbwc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbwcrwsw.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/geexmasff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gzpgaqfsu.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/glzbwbiqa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gjmrutmur.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gosqnufoc.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/ghkgbnzym.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gricegjap.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gkhpuchfy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gsnlyzxjf.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/gkmnvvrtk.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/groxoxsio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gumdsqral.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/grzzvbyjz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gvvapeahk.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gramllpsg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gvdrvughj.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gficvyxqd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gkybwnxpc.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gijatypxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gnizvitcq.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gaizfveoo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/giqwmozqs.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gqyaubmyg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gfhnanvyw.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gngbybxab.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gymkeplww.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gzhhbmino.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gszoifcpc.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gpaizbaub.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gjusaizss.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gyvzsqmtv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gbrpeaarw.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/ggcikzhqz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gnsemluvq.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gwydymgwz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gdzxvjncx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/ghrvxqsjg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.yfazqb.com/Article/details/gfylvjcax.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gqbfestby.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gwnumryex.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gkfvlsydx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/goufcpjyk.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gtihyizxg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gaplxvfwx.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gvyaqcrkg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gfjrgmnkh.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gqysnuqro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gosngspar.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gmnctyfbl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/gbxubrnpl.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gzetmkvln.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gblenasvj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gfaoploac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/ggnhdemkd.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/grxisrgbg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gsmqlaqag.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gicptwhrd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gorhipasl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gkxihnvpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gqnsomyfj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gexmrssfe.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gexvdrgtp.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gkymcmqqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gnpgszwic.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/grbbomfoq.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gdzxydxia.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/geqndrhgq.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gqphwknzs.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/guyevxhry.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gekplioqg.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/guryrrfsk.sHtML

wc -l < a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gdfdffdee.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gjhbueaew.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gxffummpl.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/grkplkqjj.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gvnmkwsqk.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gjfkwesuh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gtbewbhhw.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gryzybngt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gqhjejxdl.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gdhsnqqft.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gztbchwgb.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gdnpkjzpt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/glgsfrarw.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gwmskxlea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gylwuollb.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gfrnazbjg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gpijymuyz.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gleususfz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gwfureqso.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gombytpli.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gdplgtria.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gwciphplv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gsmohdpka.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/ghruwityr.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gbjwcpxte.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gsaeebhcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gsywrkebi.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gwbvmwzes.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gaqljvzlg.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gtuigvqrs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gcurzfcre.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gfkorgahg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gprguuwag.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gribgocad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gmrkgqhix.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/guxolzroa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/ghmzztyla.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/glrdrsdeu.sHtML


<!-- 参考信息 -->