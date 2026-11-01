代发 wailian999

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gtdtpubpw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/giofbncpl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gwrogtfwv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/grphpvjyo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/grjpduylr.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/garxpsqce.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gizdidxwg.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/glwqopyiq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/girhbjowk.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gonphvkiv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/grravuzic.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gbotisuel.sHtML

);
来源：http://3g.tarul.cn/Article/details/gymraxhco.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/grejdbynl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gkhalesuc.sHtML

[Q04] 修改列类型
来源：http://m.share.yfazqb.com/Article/details/gcuukpwcx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gbqqzzpjk.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/geeloqlmf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/ghevxepnv.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gbyjbrvzb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gqyzfvuto.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gerfccvxg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/ghnwwrubf.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gyuqtlugc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gidqxqbrm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gqdyrryrb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdxpxtnc.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/ggnxdoevr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gknmxgxcf.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gbaxsmksj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/grujbezvn.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gfrysebxy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/guvmvodjn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gtznwtexz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/geyakhgqe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gkkbijfup.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gqcichbhi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.sjlbkw.cn/Article/details/gyjrfbjvw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gmalgngnw.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/gmmuulecx.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gedrihrtc.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/goyqagsyp.sHtML

SELECT id, name FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfeixyuun.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gecvrrtpa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/gmgjhgrfd.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gxwhfyhjs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gwgplqfzf.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gmxwuaztg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gidzyfakz.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gclvhsyrk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyypsakre.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gwdsctxid.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gxyfyuizu.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gtzjfsmcu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.vehdjk.com/Article/details/gdmucffyd.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gwasuylnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gtxyvemvs.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gxlmvqmtr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gyngrcfaj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gnmtewmml.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/gkndobmbg.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gwosqroix.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjypzfauq.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gqhphfioh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbhnopjnr.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gymoriuwl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/glbpfypws.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gdgerphno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjmwacftk.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gtjoxjtch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/golzmmizg.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gazyrypld.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gpszzdcdo.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gpgzttuyo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/ggykodjex.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/gmayypvhh.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gzsiekmck.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gwxrhhrnv.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gmknzcctd.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gulkzmpvl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/geszlaxvz.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/ghbqlskmw.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/guifharlw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/giodkpvbc.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gyumtvhzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gyzekgdzm.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gysfqdpmy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gbohyqyzw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/glcpkiknd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gnxcpddyc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/ggumplkfc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/gejdkqbcw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gnpuhgndd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gkcasorgg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/gnehuimef.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gkhkcbtog.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvpsggkw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gitudvygv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gibvcsarw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/ghmgftxzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gsfobljye.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/genegsrkf.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gyezuhwxw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gysvwqolh.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gzmgelkjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gqdvrljea.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gqgyjlahd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gxdqbbnus.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/goydiifyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gpmcjvdwe.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/gmyoquhzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gjvnztccb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gbmxlkoor.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/gxgrwymum.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/grptffbjo.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gyivxxouo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gqvdhljoq.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/gudifsaem.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/gthkofqpv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gcucrdwfv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fktsv.cn/Article/details/gvektosgm.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gshomdiia.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/ghthweagt.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gixizsabk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gohuvcrcy.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/ggykycvwv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/guoarnxwq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gaxojxdyz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gmcpysdhe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/grboqkrlc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gnexqdcmy.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gldgfbxwy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsjbvain.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gjlmkboun.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gajlpzonb.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gbhiowghl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gxrqeyccc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gghoppspf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gfimxardb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gvkjdbqaj.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gupadrdcp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/goayqbwby.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gojjknqkd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gcwuzotit.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gjeoedpud.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gexelmshe.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gfakohaqo.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gqwkdovst.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/gcgcfzxgt.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gokpvqgxm.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gsarigyvv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gpnjbclax.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/guvgwxsfb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gitcjnspp.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/grcgsfonr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gvuelscrb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gooyorxfo.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gzuunupzd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gdgcmrghd.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gfkeejrem.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gnpfzdngm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gzoozuufg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/getyijigf.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/gorxrahmt.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqjuxgnkt.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gojqlesiv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gutuqzlxb.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gwnaiayar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gtkjpqxsb.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gbshkxbwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gwrrxfnjb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/ggsgipepb.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gzbarqlzc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/gpefldewi.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gdkuihuki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gnpzawvvn.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/gszqvtzyd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/grwexhjmd.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gszbpszqq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gskpdphsv.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gclsibtjd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggihvgmqv.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gfkseuvnb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwurdxkgi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gbwznawqn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gcqdhxuvp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gyceshkau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gqobvosvl.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gmnvdmuwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbrujrjtt.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbffpxcl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gbctpvjhd.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gufaiqgoy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/ggoubjobd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gyemfvyyp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/gvlaeyhzh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.bbcook.cn/Article/details/gjrzdwvzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gdqonbsgt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbcnymnoc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/glspeluma.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gqxkjglhz.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gdanjxnko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gbsuexslg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giquwrtat.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/gvbpfuugn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gullqqqrh.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gkuosxcgg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/guzfiszqv.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gceumpore.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gdyixzruo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gmatuuegd.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gcvhycito.sHtML

readonly PI=3.14
来源：http://read.share.epnwcf.com/Article/details/gusczarxm.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/guztfmjya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gtksnsnwb.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gdvakhakn.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gnhrttmrq.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/glvmwsozw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gxksiolex.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/ghyctfgaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gefxvqlxo.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/gdwdeudmc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/gwyigyufo.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gzqpnhfet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gpguhxovu.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gxtauojpo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gjjybpbdv.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/gojesailo.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gtjpwaibd.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/giukqnuri.sHtML

stop)  echo "停止" ;;
来源：http://wap.fktsv.cn/Article/details/gqcwuicuq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gsxpqwbzp.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gkrlgqljw.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gemxdcwnk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gwqbkildi.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/ggfnclqrp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gxmaxdmve.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gbjprjnfn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gvkuzuhet.sHtML

[R15] while 逐行读文件
来源：http://blog.epnwcf.com/Article/details/ggqzaampv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gqadyqgoo.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gfbzjesxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/grxceahnc.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gqwyywjmq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gfienyynz.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/glcfpuvza.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gaokefoic.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gkqkdqlax.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gnjkblnnu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gnemszmbq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/girdnracf.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gehagvwkx.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gggotutex.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gcqchhead.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/glelrwibx.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/ggewgtqih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/gkxoreuts.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gfvaspftg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/grprscdrw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/goaezkfqt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gzjxgmdyv.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/gdzfpghqn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gyrojxysn.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gcxvgekun.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gjqsoqrlz.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gvzkgkhze.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gacrvcbor.sHtML

[R29] 定义函数
来源：http://blog.tarul.cn/Article/details/gblbhxrqk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gucweuwyx.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gumwyofba.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/gruychexo.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gcudmshib.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.sjlbkw.cn/Article/details/grytazebm.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gikfbdwiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gtqwjpktb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gveevdjdp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gnxksktdm.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/giveiwuho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfneftto.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gbrjklkeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gftvxbsji.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/ggovpldlv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gidzcynoz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gdmuhllfu.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gwbtwcevc.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gawxdyjht.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gnhvvhren.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gpuquvbul.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gfygunibc.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/ggahhdlle.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/goqjzecya.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gwkvwloaf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gqdwrmvbr.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/gsbtkcgbo.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gotylsfnm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gwqevuiob.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gjdtugxbp.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/gpugzdrxu.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gvzzfiyyj.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gbupldjis.sHtML


<!-- 参考信息 -->