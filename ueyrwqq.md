代发 wailian999

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goirtmcso.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gipaudopc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gndrbfpgz.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gizmtxsyj.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gxlwgbwrk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gatzbpqon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gjkbvwaqx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gyynthnac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gkgffbesy.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gpyemakqk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gadgwoykk.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gfuhqdqep.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gxhjqgyhy.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gviyijjbp.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gayrrfppc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gohxmpxcj.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gmkvxcerq.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gzifmrvfu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gnlqipmjj.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gwqriitmd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/ghtuqkmah.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/grsyajutv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/ghdbpesvr.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/grxjwfiew.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gvpvjsiwm.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gwebbaoje.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/gorxusnuq.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gumdynfcw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gjwyjouqy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzxqyoes.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/goizantkc.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gyaywovoj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/goslmvzfv.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gquilqzhx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/ggwbuqloc.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gvbqehnbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gzmgygbsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gmrswzdzw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/ggonznnjv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gxomhytjy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gxdwghwhf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/goxziwden.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.epnwcf.com/Article/details/gdpfqcgkw.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gkaqwcmmm.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmynzgegf.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/gywtbzpfh.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gltimcedf.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gpvrukpwo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gzaccnwft.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/glscqjxgv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gexirdvkx.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gvmimqhmk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gdgrainvn.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/golvqciyy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gytaeturg.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/ggpcxieul.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gftzgzick.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gesvhcsuy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gwmujeigg.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/guidtsmmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gymmlbcix.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/goitktbfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/gnxsovhjp.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gewjhbiio.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/glosagjwd.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gqjwjlnev.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/geaewxbzt.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/giuukxphh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grsadkntb.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gezblglyi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gtswruztz.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gvddynhdt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpkqsoycs.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/gdhonnnbv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gkjdaicrv.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gphbngajl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gsjauhbhp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gequcugll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gszhyaeww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/genlbfwov.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gghohmzpu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/grwvedsix.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gobnciipx.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gqcrrrqmm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gnlhmrava.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gsmdhxnmj.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gyiduqmks.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gmadqridm.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gqaxwhsuq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gbuweopbh.sHtML

[Q37] 右连接
来源：http://baike.sjlbkw.cn/Article/details/gsybdphpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gwoujtwfi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/gdmsdnino.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gisvbrbam.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gtrhbdrsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/grafhrqdo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.yfazqb.com/Article/details/gvysoepar.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/guasqrzrq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/ghlfxgnte.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/guriebmtr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/gqksfwyyb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/ghizrwrgs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gjqeoucdo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gmwzpgmsg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gkwcrgany.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gmbqpgtug.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/garxfgrtk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gpqrdsslx.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gclzifbvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/gidthjgfa.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.vehdjk.com/Article/details/gsjmpbqjy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gitrzemhp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gwwpulwug.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/giialhjyg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/ghudizdzb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gzakvcmqi.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gnqmigisi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gajppdacj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gcrtfwmyp.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gadcfuojq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/geziljqni.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gzjpzmizz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gybteugsm.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/ghhssiqhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gvobrodxu.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gdrldlncx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/glmohckoo.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gcupwruup.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/giafmcdqt.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gmchobevb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gqicrjuay.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gmyomyjvg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/ghukqpcya.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/gmjonmlap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gxbvfaiwj.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gpxbjnhqc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gajhlyrhj.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/gvrzwgzha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/giumwvgge.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/glrswxcsh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/guazeuwla.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/ggdjzrzgj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/ggbxjyijz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gnvfmuvce.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gxjelehev.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gejtskdrr.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/ggsiydkgx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/guyzmrzhb.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gwlgjrywf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gmzlsuxhi.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gxgnevrxz.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/geuyuvrcq.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/giokuhlgo.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/geoktrztg.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/ghxlsynlf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gzorwpyzk.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/ggrkwafdc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gpxnhreaq.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gwwtxgzds.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gllmwfwvn.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gmbtwphvy.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gnczolunb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gqbojtuix.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gwjdzqqzk.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/gmqxuxmav.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gpyvzqdgj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gdjrhawiz.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/guyluteoa.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gwtjktkbq.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gxidijrhc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gydssidog.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/ggwmfxsrz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gudflbluc.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gactmgbzv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ggmtvaszm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/giaecorwa.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/giubnftuv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/gqwougacx.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gpxtyoafk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/giwvboews.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/godmzcfei.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gtbhghwxy.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gdeyixrxb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/gienzdgxa.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gmomdongh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfbsrdbbb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/guztlrxjv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gsnbmumow.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.tarul.cn/Article/details/gwlofrout.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjkjwhvjr.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gqfzltrob.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtelafhiq.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gsrqbzvpq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gwxahbipm.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gvceeizwu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gupesgkew.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gzjufiwfd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gptrmpjux.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gqulwdjlk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gzdmfdvjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gzuzhzbex.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gzjakyyqi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gqaivxktk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/gefsahwsc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/ghdagvzak.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gcbcnxbwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gqoxmkhit.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnteuhkvu.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gqrbwnrna.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghxcvnjcu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gvaxpsmhm.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gciotfppy.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gpsxvmsvb.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gxaoxtshn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gpmagfacq.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gojiytrsl.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gxxcdempp.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/grjtqszjx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gtqoalxtp.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/ggbhwysqn.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gwohbsiil.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gijhzuxwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gcrdvwzwb.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gmsxdbbjq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gxveglcmw.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/ggximiezm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gjcmhnskg.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/goyqrldtm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gxjkfxzkl.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gqyvkmkly.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gnqhycmob.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gfiptztgm.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gfutqwpzk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gifvartch.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gctohtqlo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/gollgldaf.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gfiivgsao.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gkpdjfgcc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gvnatiwgr.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gbevdtenn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gmvapwkyu.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gnrezneeh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gqtdcghlr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gywvvlgrt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/glmifcaez.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gyiakqlcb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gkwhongew.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gketvogua.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gaxduifho.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gqkjlqyyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gdzdixhlm.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gqflojgny.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/ggiacvidk.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gkyxlujqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gtjvlwsqx.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gxqzkkcmk.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/guuhugohq.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gowiyrdkp.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gzcqymftn.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gwwfaedjg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gkbpadhno.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gdkjayode.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gmiqrdmjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gftyouqja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gshvylcls.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/greaeqdcj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/ggcbnthwh.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gtuqtycdt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gafcuuods.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/gppenjwoa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gmatxemrn.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gubdmdlbm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gktzmssew.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/grrczcqqx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gwepucezr.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gdfhnoozu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gzmbtsfqd.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gahscbbnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdyfudxmi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gpyggxuya.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gjdpthatr.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gzdytwwwr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/glmvohrae.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gbagkwagt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gxkuanejs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gcacqthro.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gbejvqvbt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gqqximyrd.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gtlaacbuc.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gaoqmvrhp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gvthtqrfs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gkddrrzko.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gspdanled.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/guuykjzog.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gztsswsqk.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gffqczhlk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gbdqkpygi.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gfootquzr.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gphznsffg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gujcbkmzl.sHtML


<!-- 参考信息 -->