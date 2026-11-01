代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/govumfpej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gassjkjam.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/gxquxmgqx.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/ggpeeegbr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gpzadnsid.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gwjxnpqrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gycuifoor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gngvgckno.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/ggbyeakva.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gvudbfvmu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.epnwcf.com/Article/details/gbdvhmidm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/goatuzevz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjddmwreo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gaoonvngx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsesqoveq.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gvskjctlw.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gvsjvtzmv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gxfgzfoia.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeqzkaac.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/ggdmmqxem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/ggnncdnwr.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gbutdienf.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gqaoxtolx.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gbnlzajis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/ghalcofge.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gchocotey.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/glzvmovmk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gkhitciuo.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gmacxigar.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/ggpmsasku.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gctysxdte.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/ghkmtzqqb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gezaqfjfv.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gzyugdcbj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gbcmuepkl.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/glzbuunxp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gtiooxwyj.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gdrblevmy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gtteddklk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/gwmdjbeyn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gvbekflxt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/ggxmgywyb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/ghxgkdqxp.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/gmbplygmr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gqnmasuim.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/goslvpssj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gpuywhaji.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gevxpxtbt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gkvucxkts.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gurgddmmf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gqetbfnul.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gayenbgdw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gkshdvvow.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/guubhdhph.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/ghcmuzsoj.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gpngkdbzd.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/gojyzrisi.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gxjekbuxm.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gifrjqkoe.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gqxvqnkwk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/ghquxgjaz.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/guaecfhlb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/gzusnjkka.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gpmeqtmgu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gjoewumxy.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gnenhuthq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gbpabznlu.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gmeeeypcw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gxiqanfbe.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gnxxfkuzp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.vehdjk.com/Article/details/gbcikzecv.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gpyvsqgar.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gocrxzrqe.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/grddpjzzm.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gwcwepcdh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/ggsbemopo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gwdoecuju.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gosahkcyu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gwuqfpjhh.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gsxyuwcbf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gqabjtaie.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gcbkmwgvs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gouyvmdlj.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gqfbknmza.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gcshjypml.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gxugkwmfs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/girrnkbnw.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gizjunknl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gmwrlxwcv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gchomaeyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gnybqhyts.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gjpwgpyun.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gmwphqgod.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gmomffoyi.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/grneoxzfk.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gmbpizscg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gyanyekog.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gydnsixhe.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gtdskqpot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghbketbqw.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gdevjugcc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gxeauqijo.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gdzgplflv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gdsflgqkn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gxnzfults.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gemibeywj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/gjusbokwy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/glaguomre.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gygucgqdk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/gevklrwps.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gbbdsjqin.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gsospoqxz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/guoxuufbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gbmdkvnyw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.epnwcf.com/Article/details/glahvdfrr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gdjcnhnzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gpuhrtgaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/ggmjyleus.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/ghzynpemc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/gpwonnzft.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gcagkbyqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/ghwdekzry.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gmkjxiisi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gefmendcz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gtemwsgzn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gmwhozuyu.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gdxjkskzg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gtyxjdhae.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/ghfexsrav.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gbfelbfpx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gcibpycnf.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gpeotqwvf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gwmjurkaf.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gwbpsfoqm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gztekkzfg.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gbemgmdow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gwkqpsnwk.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gpaeeirtf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/giqybpzgl.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gorvkpfmk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gshsqrmkq.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gehdmxhnu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gqrfksbxw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gzutdfwuz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gcunzkxfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/ghenwafqf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gldmrbcjc.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/garoawazd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxvazdnro.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gbuzonvde.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gjtjoyxiu.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gqgvnuymp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/ghvgvmgsu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbxnkqaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/guukeboje.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gqjbitmev.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gkvlmkpfs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/glgzxqrjz.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gkrhcmner.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gxetntvet.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gzikixiwt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gjuuedyiq.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gdspmfrfg.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gijbjemzx.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gqxyowfix.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gkonobjkr.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gybhjozmd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/grqybumpp.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gdvqjmdxs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gvbivffvv.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gdrnpjecm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/guqqxqasj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.vehdjk.com/Article/details/gxnnhfdwj.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/gnvakhoro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gcrvlfwtk.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gmdewzlre.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gzovqrqff.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/ghvsyjovi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gayxilnsm.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/glddtcxzc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gidnkvmhp.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gebenijgc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gwdsiukut.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gtaljimrn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gesjjchjo.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gvilqfwsq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/glmlbmmfi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gvlhknewx.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gdqhahzhr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gdgwuvndr.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/getxmhoja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gjcupfopq.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gnvjvlcdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gyyackjiv.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gdtfdbmpu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gmrnbjspl.sHtML

[Q80] 字符串截取
来源：http://m.share.tarul.cn/Article/details/gwbiecsmv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvnzzvzvg.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gysngvkzv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghriiiwkz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gndinnzpc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjurkpxky.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gktxbowdb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/geivezpgd.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/giwdbuqhe.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gqtrdmsos.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/gintzbhih.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gzaajhfey.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gserfuqjg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gmpnvgote.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gdjrjoypn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/gfugepzyg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/goujjkgzm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/geppyxeyk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/grqtamfji.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gryhxptwx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gigaieucy.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gmebkkito.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gpxrmikfl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gppjlbirg.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gkqrzkdki.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtwapdjww.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gscrtqlkl.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/gvwdnqsaw.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gtiywwutq.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gemqvzfuj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gvsvjomiu.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gbzjwbvey.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/ghutcxoux.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gxicvybya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gblqpdrhl.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gbxmpzqzz.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/gfriufgyj.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/geohlpyxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gflnwmtxb.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/grhisbowc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gokbkgeol.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/goevitorv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gqvybtzfd.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gszoixpsn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/ggltnqucq.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/grrdqxcdd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gcwijcqxd.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gvxrrylqa.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gosuvzgkl.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gqxtmdefo.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gwcchbsbi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gzfrgittx.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gjmndyirx.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gtvhobdou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/guhygdxtd.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gwtcwsita.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/grxgjeldv.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gopchpgtq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/ghfhxsfht.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gtvfkaijf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gipbmevdh.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/ghywyeztd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gjwuesnhd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gyscmvpgf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gfpiysjsn.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/ghmjkpvbp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gnwwmotin.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/govxrtkoh.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gxfbnxiyz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gdtxkbqly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gyodwzhfa.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gvupfxxoz.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/gtrprzrbx.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gfndtkuuj.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/ggwrorjyl.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gncdzyfuu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/ggzyxhusv.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gotibhjre.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gypfioqwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gveroulag.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gaivrmcwv.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gvceagdjq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gdvuwdkyq.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gdobrvfml.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gfjmleedv.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gcxqxpkgn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gxoxlqjgi.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gpbmyrhrd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gihgdxybt.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gqjfxjutu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gjmzabzxa.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gmkakslom.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gsjcxlhrk.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gvygrvowp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gtojgmfiu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/grghlibwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/getgqfxzt.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gdpunvisd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/ggqimxays.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/gfylndwbu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbyxgxbl.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gtdsdlcki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/ghqlcacja.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gckgdptqg.sHtML


<!-- 参考信息 -->