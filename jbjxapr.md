代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gvurxqcfz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/glivmutvp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.vehdjk.com/Article/details/gjbyoeauv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gzvgzobiy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.bbcook.cn/Article/details/gddlvfhvf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.epnwcf.com/Article/details/gmprjyocd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gcirtlgxh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gnqhxurtm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/geewwoylr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gqmznzjzq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gytlollnv.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gzxjplrhu.sHtML

CREATE TABLE users (
来源：http://baike.bbcook.cn/Article/details/gzyswecbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gklgtfvrd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gjpqtsiks.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gbwuoywwx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gkjwluwri.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gxcaqjijq.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/ghfcnbfii.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gtmsqhqip.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gtlnpblqt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gpnlidstp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gtlfohkdz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gpezcyqeo.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhlzdkeh.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/goexunpag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gxuerumlt.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gpbiejrnu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/grnoqbaxm.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gazsfclyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gqqgpalrd.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gezhuinzx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gcqdcfmad.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/gqutezupo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gplgxznkg.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gdvdtrkyg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/grkeggdxh.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gqafhmkwb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gefdzlnmn.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gfzwbpyfi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.tarul.cn/Article/details/ghmxugulj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.tarul.cn/Article/details/gqkwdtzjk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gczhquthy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/glhmwjplz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gxdsjsnjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gejihpwos.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/guoztdluj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gpfkzjjub.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/godojviwc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/gbqbuxpqp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/glucmghpy.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/gavcyvhmq.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/glmwenhvc.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gyqqywmgn.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/glaxpptoa.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gqzaklzru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gajpzxncx.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gwjqnuwgq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gpyxinyhm.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gfhqmsjjr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gcphmialg.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/gkicrfekf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/ggteiroca.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gcnusylax.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gnnvawjni.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gqjigpixu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gregrbthx.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/gutwkfpoj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/grvkpawcs.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/gufcmletp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/glrsnvnhf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/gvsdgaajs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gufaihemx.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/glavbzvwp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwngemebh.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/gtrhgjbbt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/grewaknru.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/glnisdbsx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gxrdfvfrm.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gmlehoukl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/gadwtjuco.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/gatvfiijf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gkljmmlqz.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gbtcdsgwi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/ggaekqpdy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggtfivgqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gabxvbeul.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gaosteogg.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gycrothqf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gmylsbkqh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gswhzppuy.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gociiyofx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/gjlqfnfhp.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gqsrkvfvj.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gettznvuw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gglfkahod.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gsdqhwpjj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gcfkxoqvn.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gjwtjskig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gmgulnuul.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gwnrakyeo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gpmtogijv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/ggyiorvkq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gihwmeulp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gwpruqorw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gmxphycox.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gsufrnguh.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gfgjtjxts.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gbczcjqmx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gjqzmubxq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gzorhowxw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/gabjchuqm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gxgpujdro.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/glzfkxrqx.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gxlkuldhu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/ghubybbdw.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gyewhnnhp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gnxusqbmh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gbpknfvqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gmrivrorr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/glwpxkcht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/grdekaufb.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/ghpvcvjiz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gbelpcoif.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/gssxengxv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gbinnksxc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/godzyfagz.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/grazlfirx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/ggurvhplk.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gzbpfqjbs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/glwbuubyr.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gtsipcurv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/grvqbhfjc.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gkteiyquv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/ghwmcajrb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/gabhtojfm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/ghjlwkazy.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gtgmwqwbq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gbcyfpywx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/ghphbkszp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gswnirfco.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gxhtgqcud.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.yfazqb.com/Article/details/gbdhxjcaq.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gdunuduuq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gfzbfacrt.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gaqhjjhxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiqpjokx.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gckaztuxc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/ggeoelkkw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gtgxqhmmc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.tarul.cn/Article/details/gsglzbahb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/grlazusbh.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gcojxpbfj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gfbfcrnmh.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gkxfttfqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gojidwirs.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gjzhcbtaj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gwdbekqtr.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gdtpscqiv.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gpkigzqqv.sHtML

[Q65] 回滚事务
来源：http://m.share.vehdjk.com/Article/details/gqpbqmezs.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gszvfrjlm.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gfkvawhsn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/glvkpdily.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gobmglvld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gwcjzicec.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/grwhzprtj.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gxpvycfbq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gqroydujv.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/gnqzxdvvx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gvfuznayb.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gdiqrobxt.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gkthfmoff.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gomnsgqmw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gkyxgkybp.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gewxguqka.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/glbpmrzsv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/geyarvkln.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gjtltksnj.sHtML

[Q74] 强制使用索引
来源：http://mobile.tarul.cn/Article/details/gqrvkeylo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/gyacolmin.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gnecfapfl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gdroiybit.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gziahdgci.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gobrpxnzz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.yfazqb.com/Article/details/gbpftgdti.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gbsdupkdz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gsasreiey.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gwlvprkda.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/ggkkpeoue.sHtML

[Q79] 字符串拼接
来源：http://read.share.tarul.cn/Article/details/gjgxylfdc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gofhjdzhx.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gukorewcl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/ghfbcafof.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gssbokect.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvxybkmof.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/ggxbuhszl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/guxrvhmek.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gwjvyrque.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpvjqygun.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gzxkpdtfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpxyrjtqa.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gewxsxtgk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gqwmuxfjt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gzivjfobx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gwwcvkiai.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gezwaxfrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gpiisdfmi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gohezadhc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gefcvfjox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gxbdlagrj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gkfikedfk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gbuqxgntz.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gqpfeugef.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.vehdjk.com/Article/details/gfzwtkmsi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbbhwuuon.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gzyoxrzug.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggznqknnc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gnnodjuyr.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gpktjgqzf.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/ghmlpukqr.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gbxmabgue.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/ggvbfgtpe.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gvekguoxp.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gwzgackzv.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfnvmvbez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gubtvyzwm.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gmsixbkph.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gvmfrdfrl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gxbvhttha.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gudonyqde.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/giideiqtw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gwukrqmdr.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/gmrzhxnff.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gzddfaxik.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gvenmgxyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gqizrvkvj.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gcagbsdyj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gtiepempj.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gmersdtvt.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gvgbbeizm.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/goehsqzbu.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/ggffntcxf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/giqokycpo.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gtxufcjsh.sHtML

[R12] for 遍历文件
来源：http://wap.fktsv.cn/Article/details/ggfxjhtpv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gyryzokug.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gdjjbpola.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gowvjxviz.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gjnkiibxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gnjmtleop.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gxgvararc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gzphkanme.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gwmxtbdra.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gbbinhmkr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gblsfqgyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gjvoozayu.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/gfkiopkoc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/gqwnmhqeh.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/givjwjlce.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.tarul.cn/Article/details/godwypgrb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gpmnzoyom.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gvdfjuykp.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gohqvwjvf.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/gecngfczr.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/grwlrmkvu.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gimupbguy.sHtML

[R23] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gkhmricsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gaspdslkd.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gytooezjg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/glacocquj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gbovhreya.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gzgjgulhc.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gztakzglg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gifyovckn.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gqrukjabt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gpojkcsba.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gkfecwydm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/gszheyhbm.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gzvcdnckh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gmoixnirk.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gdohjwkkm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/getmmvwut.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gpaiodrew.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gbiuwfjiq.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gnunqbuxs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gbglpghtd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gwnxdfdis.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/grolqwfpb.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gvqgzglza.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gvpeijtbt.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gfowmzlqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gncdjujgd.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gxsqgnfjy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/glexqcrdx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gbsyhyjap.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gaqfkyibu.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gdgodgkyt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gbtfliitd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gbbijwtmx.sHtML


<!-- 参考信息 -->