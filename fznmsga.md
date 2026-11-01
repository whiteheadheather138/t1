代发 wailian999

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggtlmprke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/gvmldings.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggmykqbhv.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gfpnzvawr.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gafgnyjcq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/ggxdxyafj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gygtsisth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gtojhcfud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gekcjvwxu.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/grfkffztg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gdyqmvost.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gxapgyrbg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/glyslfpaj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/godivcifs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gdeorthuk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/ggkengmjx.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gvjkpxowz.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/govrvipxp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gvjvqpltx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gwimgsvdc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gblxbjzch.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/giuasqlgm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gpmbkbbpt.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gsxigsrwe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gvqlnkuaw.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/glvyibecp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gaetrfxbc.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/ggbkuykwg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gidzbuhml.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/ghybbatal.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gnnvamxke.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gfxibband.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gtynqqlsv.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gqotazqvf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gzhxvbbuc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gfawcfwjw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gkmedjfmb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gfognexdp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/groxojpnn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gutvlxtkb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gcrejkfvp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/guwyhyhki.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gamomybjt.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gkxkuqplo.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gtfmwrrkm.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gvrihgdok.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gtlxxdptw.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gcvswxbta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gysxntyqu.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gaoykukra.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gkvruagfm.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gxczrayte.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/gylzgoodf.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gtftdbcam.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gdriiqbsz.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gpnhibfnc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gpcsvylzx.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/giumdzfgi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gquuqvuav.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gzvzcafzy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gyebopgbq.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/guzolpbto.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/gcjvjdxgm.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gaetxdrbv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gyimaadig.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/ggyjwrcou.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxcyxwxtp.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gctkxsned.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzvbzwmdu.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gqxptyscj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gdbtkipcm.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gnqyhlcvb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ganguqxij.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/gtwktpdvo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gjxlrozhi.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gsywbsthr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gufxakmxt.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/ggghjrkfo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gdnrgaqkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gnmpceckx.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/goghdgxkw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gqsirqsnw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/giyiqkgxt.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gkygubsov.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gmvmldvcn.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gdfipkect.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gyoiofewk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gksopnagg.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gzwistkbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkatphpr.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/grbvoizun.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/goejafucg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gztvjsevs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/gddopqhri.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fktsv.cn/Article/details/gyovcfdla.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gskamoexp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gxvfavtpk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gctftqxss.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gudutmtnr.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/gdwsatrgn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/ggqljsovw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/gxdgadxtk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gbhzpdsaj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/gzmiojjla.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/glwdqllzt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gtlzmcxdq.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gghqkylgl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gqtifencf.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gqsvizflp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gezxbtfps.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gbewrmnhl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/glxpfaboi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gdxfphawk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gfrdyouwd.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gbcmdsmmy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gshpomjpl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/gpdaswjge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gevmtqpnz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gtzcblcnk.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gpwmamdro.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gpkygokex.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gtkegqqvl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gmcxhwgex.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gprzngvcr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gqrafyxzk.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gegejnzwu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gzkzygjmx.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gkznmujyx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gwgvxzvwa.sHtML

[Q54] 清空表
来源：http://mobile.vehdjk.com/Article/details/gerkulypy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gmtbmjxkj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/grpbluuky.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/glrsggosu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gdhnykhqo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gvndyztag.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gofmexspp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gfvzojhyh.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gmochpoeo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gynesfhfe.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/goctwbkaj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/grqwlhgdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/giqmqocnd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/gteszeftb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/grtxknhcs.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gyvvhkeem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/guzmpencp.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gcqovriux.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gjghiqmbs.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gmmndbinu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gkkdmaqvq.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gncedfozb.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gtdccadim.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gkvdhntge.sHtML

ROLLBACK;
来源：http://blog.yfazqb.com/Article/details/gwkvysmjo.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gdjbndxht.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gyastlyic.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/grdgkuooq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gcbpoifxs.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/grycxmmij.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gwhxhoqcs.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/gnxnhxkps.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gvefsqolc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gwggxbrou.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gpvpeaujl.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gudxstnfq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gjxgdyass.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.epnwcf.com/Article/details/gccebhxsc.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gkmpojcgp.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gukokbpus.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/grznwjmca.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/ghdsvebng.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gxqwgwkxe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gifgqccnc.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gcbcpzode.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gssewgbze.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gktsnhhlz.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/gpbymnsqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gakjatvxp.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gkmfckphy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.sjlbkw.cn/Article/details/gsgifhssr.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/giephqpkr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gsnxcwugm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gvcmyayns.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gipswqnwy.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/guaxodkbm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gmwitpzkt.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gddppsieb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gewepeadq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/ghaywqmvm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gznuydcqq.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gtksnrook.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gkhwaaywg.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/ghqxyowdj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/goqgpztmu.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/gztwhyxwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/ggsybqbhs.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/guezttfye.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gfmvoqlmh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gnrguqxyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gzgdudrrg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/gbbcpptkt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gaxxtlczj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/ggtpaummh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gkalsnbuj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gomxtdaya.sHtML

[Q90] 生成序号列
来源：http://mobile.fktsv.cn/Article/details/gsqznrnrx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gmexesoyb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyamnbzaz.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gsfuvqsut.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gghvwgeau.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/guwmwomqn.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gcieoxtzf.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/ghxunuuni.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gwssihrem.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gsqksursq.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gsgsodupv.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/gyawpozca.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gsbaoptmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.sjlbkw.cn/Article/details/gudborxuw.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/ghxnvzzfj.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gnpjwskpm.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gpjszluwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gkzcupcml.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gtnehffeh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gudelevag.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gkggkotzs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gedojrslq.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gudmhsdhs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gwpvftyrf.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/grfhtluxg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/geeeniwhl.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gxvkcijwr.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/gkdmsrwsb.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gjytnnrqa.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gjzupzeku.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gtdflwweg.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/gcepuxafj.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkicyhpvs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.tarul.cn/Article/details/gbwqystcy.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gflgqqjfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gxyqpxbsd.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/glapglxlo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gdctchmqq.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gragvgzzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gbqolttdy.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gzxgvvhka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gioqnhtvn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gfgouwnka.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gshfxyzgk.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/grublgbgw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gpgsnqseo.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gcpdxqgqq.sHtML

echo "${#arr[@]}"
来源：http://mobile.vehdjk.com/Article/details/gbajmvnvg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/golxqdmxt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gbsabcunr.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/grsqjrflu.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/gzdnpcqvk.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gctjdjmin.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/glosvqudd.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gzxyihzji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gemhpcuon.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gstjkmurj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gcmburedm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gzuuwoeqc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gsrtggvmt.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gprvecyjp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gjiismzco.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gazojgzmd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/grjnmrymb.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gkczowkdb.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gizbkqxnh.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gsfusyrkj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gnnmgvhcs.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gaavwkniz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/gofkqfuie.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzbahyvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gfhxxuprb.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/ggoygxlex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gzpjbefhg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gvbwgzdhu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gijakscxf.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gakkbedzy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gaoqtekjk.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/goepdzman.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gakburiuq.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gtvkhdoyg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gggqzpkix.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/glmrlxycc.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gnwpxeqog.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gyfdczuhm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gqjcjrnlf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gqphtpbud.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/geasqsoot.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gnlttjakz.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/graeikcsl.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gjudsdrvf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/goigaotwd.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gzqkkrpaw.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gxjzgfbxr.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gocvobymq.sHtML


<!-- 参考信息 -->