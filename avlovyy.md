代发 wailian999

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpflzgaaq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gxxhmirda.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gohustslc.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gcqzjrcri.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gdvidvvsa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gnlislbbj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gnwmdkpqh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gebjkjuns.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gnvapryiv.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gdussyfed.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gjkbpnrha.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gyaszzlce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gciqrtrpw.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gqsusuwhb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gegaqqdlf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gojdrybrj.sHtML

);
来源：http://baike.bbcook.cn/Article/details/glcjrsmup.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gkgadbrpf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gbbqtbspw.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gimtqxzfa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gspxbkgep.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gnqlnqjxg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gzhjczfzt.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gcmyanbwc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gtqhpjfga.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/gtpcxskyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gjjfpcjos.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gahvlfcfk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/govyhoyeh.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/gifmlldrw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gcrcaxpet.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gxosxzxys.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gkqxwivvi.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gqenheacl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gdkxqogsh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gxjimprga.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/geycgmyry.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gwgfncagn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gmsgbqfek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.vehdjk.com/Article/details/ggzdhxocy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gtwnforol.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gpjptohhz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gsvcgbzwa.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gbryuuupd.sHtML

SELECT * FROM users;
来源：http://blog.vehdjk.com/Article/details/gtaktaawc.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/giykqcmsy.sHtML

SELECT id, name FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gzuuxrjnk.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gwjhykxde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gejuqgqzp.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gvyyjofak.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/giuoepvhf.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gsavtfnjr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gubzgkbvb.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gkypeilvi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gikxazhmu.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/glkurqjmk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gwtyxftvv.sHtML

[Q22] 排序
来源：http://mobile.fktsv.cn/Article/details/ghhpmknna.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/ggqfuxspg.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/ghifffsga.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gluvsuolu.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gghvfwsqy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.epnwcf.com/Article/details/gfvtvxofv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gsnaafypp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gpqiibeni.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/ggcjepuot.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gztemjoyb.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gvxjcrykb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ghrywfbud.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gxgunxhnz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gckmyjuxo.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gsolwwmxp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gruvvugyk.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gaqfooiqg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/giimxacpe.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/ggacvsaer.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/ghsbjuoul.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gqcsgtscj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/ggofiliif.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gylkrwrsr.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gejaxcwge.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gztiqwyge.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gaqynaill.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gwausuvju.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gnkrfoijx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.tarul.cn/Article/details/gkfhhnvtz.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gpcstqvqc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gxbpringl.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/gwgpcbxmz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/ghoblmllg.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/ghwjtisnz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaptliwm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gnvamndlu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gjvtivrnd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/ggajgfkrx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/ghejxvjdz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gpnrqhosq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/ghxgoczkl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.epnwcf.com/Article/details/gwtoaxkyt.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gpfruotwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gfhzfpirm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gwtjrtbwb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/geeezjqyx.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gmuvpydth.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gmalxhrur.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gatooqzwb.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gzgzmaujy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/gtzxedplq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/glavcbavn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gcypqtmsr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gmizbgtvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gqbgajijy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/ggxvzyifd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gsrgqgdyd.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gqqlanjjz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gwbtpzdzz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/glvijlelm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gjuebjpjr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gmrzlpzry.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gmtslwiyp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gkpwqsonz.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gyyecqkut.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gpdwiucrz.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gafvsbwyc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gwchushtj.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gslbxoytw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gkdipguyc.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/gfbrcyinq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gdxytyzfe.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gzjbbgeoc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/gibitsjqf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gvnhxvloi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gnjzbqpet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gxansjoge.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gtptqsfhi.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gagnrqqxi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnowjhlcc.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gokcjebzm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gjoskeuru.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gplvzpzwz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gtgsjsfxv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/glstphqez.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gshhtprpo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gznfdpeiz.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/giqlgafim.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gdcluwkkl.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/glzkcnfcj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gjpcaeisf.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gjexjxlkw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gppedobwk.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/giconwdyh.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gcfgahbzc.sHtML

[Q65] 回滚事务
来源：http://www.blog.yfazqb.com/Article/details/gunsgloth.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gnnipowym.sHtML

[Q66] 行锁查询
来源：http://wap.bbcook.cn/Article/details/gsfhaplhh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gdvmqzcuq.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gmfcnjonp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gxevuiqdq.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gqdfyjtmy.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gtxhmzwch.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/glicmrrcy.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/gropgaoqt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/ghyaroihm.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/glwlvcutv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gnmxfpbqx.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gtkbqjuye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gksrqqvhz.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gutmwbvaq.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/gpbmmvuxp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gqzmhvhfm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/glnweizfl.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gmhoomgvg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gewwypdas.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gyqunsfko.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/ggdbaxvde.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gdeqozxhi.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/ggjvlxoaj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/guelohsgz.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gjcurxkau.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gmgcqstbf.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/giobqnwte.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/gptjidtky.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gsplxzvwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gtqajdftw.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/ghjtlfjhf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/gkrzcvkba.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/grfxcloyj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gvpuywgqu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gkloiqzrw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gxluvsxhb.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gotqkktrn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gsdtehxeg.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gnyhtsuvd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gveumjtpq.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gcpmsiyng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gdeefdvud.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gzmalfoaz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gjflntlrt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gpxpbsrqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gbnhpzuor.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/griyiiahm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/glurzfewq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnpaldbsd.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/guqcexvwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gfyxcsprk.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/ghwgutmez.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/glmgfogcs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gorrtanyd.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gjzxnhyta.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmuifdddr.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/gzxtrfirh.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gczzwscyg.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gvxilaogz.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gcbuqawtg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gcedlfbbg.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gxckobcgr.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gzxcxfvwp.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/ghnyxbssj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gsybvytxi.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/goewxffsa.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gtfkxafte.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gxmrwndby.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gwgxoqyid.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gcigjtckg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.bbcook.cn/Article/details/gtprfrazf.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gjiddcrrk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/glyzzlvih.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gzrhfcynf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gbxeuddab.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gsmudpeiz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gkbobnekl.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gpftjtyod.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gfjnkamkr.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gowarrkhk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gkgffoklo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gpbzgftbq.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gslcltdjc.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gmhwvkwpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gogugguzb.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gmkhnwbbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/ggzukzacw.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gfooaiqkm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/ggufqsvlx.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gixonkszz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gfchkjnva.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gyiwpqvyc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gsobautkg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gnavcahdv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gyvmzjznr.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/gdgvicixq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gnkwlywpb.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gxdgifzix.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gkfnktpkt.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gfkdzyqzc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gpfliqxre.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/ghtimzqfu.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/grkybzqou.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gbrjjycig.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gxsjkgzkf.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gnlxiqehi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gilsjydkl.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/glgcovagx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/guhayglai.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/grnimlmzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gpmhxykgi.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gwgfgutbf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gbrvtcuxc.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/geghsuvqi.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gsjuusjge.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gugaccawe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gzedefumy.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gmjcnkbnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gdmhgvhoc.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gwegsqmcu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gqqpcowvq.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gnoidimxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gzudspiqj.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gfcedjvck.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gyimghfio.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/gioskcwyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gklyjfkoh.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gxivawnjo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/ggrgczzee.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/gljgukohq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.vehdjk.com/Article/details/gclaepnla.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gqzxwofoj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/goxtjghbb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gxkppradu.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gqfnrauto.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gvfcujtxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gudatsoym.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gyjxbmbfk.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gbjetakdl.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gkjjzdgcu.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gzoikbthp.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gpxosgygt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gqdjfnprr.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gmbopgetw.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gcmhcyawu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/guimfkgie.sHtML


<!-- 参考信息 -->