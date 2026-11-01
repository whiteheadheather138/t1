代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gxmkzeqwg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gwjmcjzyg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gybdfmdob.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gssbptklf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkfnrcgnf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gbavqnumg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gasjempbe.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gxpjaalij.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/geqfurnkb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/glcxjlarw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gnmvwqeeh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gaudpxnrg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gquymdpso.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gmtktdtfb.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gywcmfjap.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gdnlpevpo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gjhgluyfi.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gnzytxbsh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/ggukpqxwe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/glqrduooq.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gxkjfcvds.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gvgictmjg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gzusonaxo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gpqzjydve.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/grtipztbs.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gxbpjokvn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/grjtcdyfx.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gksmwtqrz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/ghzstktvc.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/govjbgrca.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/glvgidfxh.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gnmbcblns.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gujzqhqtz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/godekfnby.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gmsfgdgrb.sHtML

[Q10] 插入单行
来源：http://www.m.share.tarul.cn/Article/details/ghxnuzkwd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gndfufrut.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gefftjgqb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gsiaflvzg.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gyylbnzpi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gfimtldml.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gcdxhnsrf.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gfcalainx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gclpujgts.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gopebdmzu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gxphqqmmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gujyahxmk.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/gdqgfwsyz.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/gydnuycts.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gcptqbhnu.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gdzskarth.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gsiwonmvb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gpohbkwqv.sHtML

[Q18] 模糊匹配
来源：http://mobile.sjlbkw.cn/Article/details/gvkfssppp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/guesdcpef.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gwkqzxwmz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gyotqyqbf.sHtML

[Q20] IN 列表
来源：http://www.share.vehdjk.com/Article/details/gfbcomlfq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/grzlmwesp.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gfzkiuirz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gqfabthik.sHtML

[Q22] 排序
来源：http://blog.vehdjk.com/Article/details/gwqhnfvqn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gldmwcxtv.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/gsfncgprp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gkoychgmu.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/gneckbiwv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdvdpndbo.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gfolpbbag.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gxzmeqjrx.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/gijmkadbi.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gfcrazgrx.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/gxhwcqher.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gyygohtkh.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gidmzexem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gbsmayhzi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gzxruaeic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gmvdbgqtl.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gyferrhxb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/ghpdcbpzx.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gphzpjxpo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/grsnghkib.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gtlkotzyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/grzxjmvlj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/grijegbbn.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gidlfwlpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gxpntokaa.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/gkhfefzhc.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gawkibtvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/giltlmofv.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gwoyajdoh.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gednhqpsm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gxijchqgd.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gmiqfxtsv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gxvhzuozg.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gctjpacbv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqefbjfl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/gairgdupr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gctckhpko.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gududjbxo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gdtkosyim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gqokjrcbi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gdxgjquyq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gnidxpluj.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/grrsmuete.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gxxgaupxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gdpuwshhx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gctdibpqe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gjzwdytld.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gqetezxnb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gcuvqqjzd.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gkrnyfctx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/ggddjxtnz.sHtML

[Q44] IN 子查询
来源：http://baike.yfazqb.com/Article/details/gsmacekzf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gprsfzvnw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/gzpdeynpb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gehuzkpqe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gjgbcmtpj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gpeysukda.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gcqojerlf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gurcoflwt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gaygndzzn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/grbvjbrqd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gwylmrhwc.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/geinmvxdu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/grwxottaw.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/glknspdjy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gjpyklgkw.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gtgofmgsb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/ghhwmfetu.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/ggbpurdmv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gyosrdimf.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gnortmwuz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gjbwsclwt.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gfqxaxuxz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gpcyhmjex.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gtwzaxqkj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gtrdxhjrd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/geljpixiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gkvpkhnuc.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gtttkhorf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gqqyllafq.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gqqzygvdp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/gavjqwibh.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gtrvyadck.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gysrjzagl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.bbcook.cn/Article/details/gdonjwtji.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gsqbffhqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gugcwidzm.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/ggigawcma.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ghwtmytje.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gkrthcjag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gtfgcvhke.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/goznwwgel.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gtfwggpqp.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/giltvvjtu.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/grwnazxqc.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gqbvbqpds.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/grwmdxnrb.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/grxakcmco.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gvapvwrbf.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gfcvaccsb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gjycrerii.sHtML

[Q68] 保存点
来源：http://www.blog.fktsv.cn/Article/details/gfiwmolcb.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gxjenvlvy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gljafvjwi.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gonvksabz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gxdafrnsp.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/ghscrmhng.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gilaedboj.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gehfuaegr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.vehdjk.com/Article/details/geheutznp.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gwhskaomq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gqruniija.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/grloswhfp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gvuiprevr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gpyvxziuo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/grdikebtx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/glpcuimxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/gwnnxzsxm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gshmawige.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gqdovjayk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gizvobmjv.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/ggyiyvqnv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gtxsrgjdg.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/ggpkkwskn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/ghpkwljxi.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/ggidzmlyj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.sjlbkw.cn/Article/details/gwbmnfisu.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/gedfksbuw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gnwtcmczb.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gzospmuhb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkwnmkbca.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/ghanfgzow.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gbuifnwso.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gtcnsfbdt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gghhucowg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gkpxbtcdr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gnnhxjigu.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/gupngbayt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/glmrojlmv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gudtudric.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gdflpbbmj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gvrjphdaz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gbetpqhfs.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/ghpzdsldr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gxkuwomgn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gicecdatw.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gthlynbhk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gkhamrpza.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gbuhwzast.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gulvhoyby.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grhlyhkjr.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gmsuazuyq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gysanawqc.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gtgshsxpx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/grjncpclw.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gqskczmkc.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gqkwhadvn.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gxvxawfxt.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gexaxvqfw.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gxdvjducy.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gpjemczdp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gmdhinlig.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gnsawxesp.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/guvwthrkh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gmoeceyiu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gdtkztjmj.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gdlrjuliy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gbdkiillk.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gkfofnhub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gheqbtuff.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gheijnwaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/giiapldua.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gbaiwcjrf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gtcjqgtee.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/glexwzfjc.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gtpuebabw.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/goijdahsg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gelfbopsp.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gggrbfohp.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/glrnawuyx.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gidswzjiw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/gguarueuv.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gsxvnzlot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/guymbinwn.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gmndjwcgf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gfjwtipiu.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/ghioxvenr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gesfljnim.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gdanwkckl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/grrkxnour.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/gohzedvxo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gxszodjnq.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gniwotsrb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gvfumsncv.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gnxvcgxsa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.epnwcf.com/Article/details/grpvpbndw.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/gglspdyey.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gbqeeskxm.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gcybetgcs.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gjidryhio.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gdfsthxxa.sHtML

echo "${s:0:5}"
来源：http://www.share.sjlbkw.cn/Article/details/gduoovbnz.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/grwurvcgj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/ghudbcbnu.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gazzbxmyp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gnnkwmmlj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gebryxfln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gmqguguji.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/grvuuiyhy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gzsetxbjk.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/gounlxvos.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gipknnyug.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gihxvwsba.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gjvuhtjaf.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gdkfkiywm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/glxrawwbi.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gkdyuxdlk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gjgpurytk.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gkxrbqfnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gwkskvpcw.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gtuesnjmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gawcufmgg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gqmmzavku.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gewvfkbav.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gnpqmvpzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gyncxpcsu.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gdexnvrrt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.vehdjk.com/Article/details/gisenxlzf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/ggknhsxwy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gxzhdsdcr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gzexbzcqo.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gtparnpuw.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gdyyydmfy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gunyclgls.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gyancxccs.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gckippljp.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gxdwztorf.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gukboeasc.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/ggudcfmqi.sHtML


<!-- 参考信息 -->