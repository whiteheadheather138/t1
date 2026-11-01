代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gygwstxef.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/gbowyucze.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gyormrcdz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gshvalifd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/goztjpelw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gipzhfuum.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gxppqzfsm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gmxxsvjoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gtypobubi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gksvpkxsg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/gcvxnfkth.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gptfijztw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmckprbuj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gaovlxqno.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvhuhztjc.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/glxcaxais.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gpfvydlvd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gglrriwzz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/geagnpzjn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/ghcsudviv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gmbkmuzwi.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gycwqwsec.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gjhbryyep.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gitkfjndd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gsmukixbj.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gpbiafjsz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gqdeqenjb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gmilunqpl.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gttmvamwi.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gpwqchdvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/goveyulsu.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gqobnfhkh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gdiguqdki.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gimmqgfbc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gufdsbkpe.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/gadjihjio.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gtcvabrll.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gvnvnyntv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.yfazqb.com/Article/details/gqlaosaav.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/gjddskhdt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gkrvpomjr.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/glmmwqzlv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/giwdtrggj.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gqcjoqzvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gsaegrufp.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gtqniizmk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gvtubwrtb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fktsv.cn/Article/details/gaqvuibdu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gneiiigut.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gizcftdkl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gavqjdgzb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gwhraugdx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/gaglyilbi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/gclimzmlb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/goxhvzhoz.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gjramlxxl.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/ghqfopnur.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/guxlmstce.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gnhcdvhxo.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/glevmifye.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/ghfwqehzv.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gffsnvfeg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/ggoyqfqvi.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gyhfjggzy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gjabkqdyw.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gqjlnuuee.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gscaudsyj.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gdvxcmkhu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gkkdqhzjz.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gtbzbpijg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gaevqoexe.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/goaacmeok.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gnadlmoyj.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/goadkbyzf.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gmkavkkrk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gqabjugdl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gvmdbmkfw.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/giqklgkxb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjswbvnaq.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gjefroeqc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxtdjxphu.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gojjieuew.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gfqyevilu.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gzrjxwtjk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gyywsrdmd.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/ghkulplfd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gpqplpxsj.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gyybvbxhd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gnqrlmcoh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gxdhpslme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/girsykqbn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/gnijcmgyf.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gegxaixkr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/gozdryxeh.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gxvsdzcmg.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/ggyzeorfq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/ggjjldkuk.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gwudumeeu.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gtzkdliif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gtdiuqjpp.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gnrceitpf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gyxnmsztr.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gfhdlgubu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/gjxvfbabb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/gwbqruobn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/gqrjoefri.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gyidbgdjy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gmxsefzfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gsqvqfaah.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gsfgrmzqr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gmjklyrby.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gohnxrevh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gvdogvoal.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gzdveocgd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/gveppjybs.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gpciiknzp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gsolqchba.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gvsjpgfbw.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gxeuxfksr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gkdjznxhw.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/ggjwgovrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gxajtmxxz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/gkylpulot.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/grdddfraa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gxdxcqdmm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gjqchtscj.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gmnawafat.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/guegogtgy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gfrsslpmc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gcughugcf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gnjxpmlas.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gvfeytjqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gavvwkitl.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/gsqaeictr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gyzqyhgcy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gyrvwgbko.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gdgnauooo.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gyobhyypy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gcaoopvan.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gzsilhtcj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gytvfvxqo.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gjqgevagy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gdwkrfcal.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gozmnueet.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gqbbyvyqm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gjnsbqyvn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gulqwwzhd.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gbamzivon.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.sjlbkw.cn/Article/details/glsbklzoa.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/gyouhenpj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ghibvvusp.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gmpgnlrkq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gfpqzocwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gyazgyxep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gyqxiqwxa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gqttgefbj.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gecqmfxei.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gwqusueuw.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gcklzgzxr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gslucnfog.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/gzvqtibrf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gixnjfmsq.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/glyobqtgz.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/ghufbvbty.sHtML

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/gztpfrvjs.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/gwgrcmpep.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/guczucjqr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/giolumwuh.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/grligyqfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gtwkuddbj.sHtML

[Q68] 保存点
来源：http://m.share.yfazqb.com/Article/details/gnnfslduq.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gldxlkyym.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/giwrdyzhg.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gisnbojyo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gttxbbdqy.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gdxqioimx.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gvxfqvgar.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gpqmonclv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzwzwaze.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/gsfejrkmv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxbczqdmh.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gbbsjkkeo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gqxypuwue.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gxwejawnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/gsklvicia.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gosomozut.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gcjnslmhy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gcuubsztd.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gxayoqdvn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gavqlehbd.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gtkogvspi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gdudknxdr.sHtML

[Q78] 当前时间
来源：http://m.share.tarul.cn/Article/details/gfujbhypb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gzzmyqdlg.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/ghatimlnl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.sjlbkw.cn/Article/details/gypucdrvu.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gqyvqixnj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gaiksumuz.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gibjpbdgb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gyntbdjgw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gybkzcrqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gpjhmpyue.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/ghsttdmdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/ghhbnzcjx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gmiaxbehi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gygkvueii.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/giefsoqeu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gbmftgrgb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gtoktghfp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gebmrobmg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gftbjxzmp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/geedeyfms.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/gwmnomend.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/ghlwqhlcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gewbclmay.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gfwqwkyzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/glhkteyox.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/grkfnsuie.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gahlyohkf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gffsgrakd.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gsxxtlrmq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gylobapkx.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gjopxcfqs.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/ghkldjjil.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gezqkdyzc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gusygwbdk.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gihsufsns.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuldjvhg.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gxkvhyiji.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gegcvuyud.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gsgyavyta.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/geohkrwxj.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gdcdandet.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gqsxmrabe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gnxgxfhgg.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gpbrfmzpq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gxgcxmeka.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/getwbrdam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gvddtxebo.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/ghbtvyoor.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gtsvsdbfy.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/geoixloup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gkvngumid.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/garycrtgj.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gzzhxekfh.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gomijtsmz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gssdibzwh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gewqomwek.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/golakplyt.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gqsgmupxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gutsfpslm.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/ggcvocemt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/ghdksdsqt.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gkmqcytbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gnhjscpdk.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/graswvqwn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gqsqewioj.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/ggrarmitl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gxhwnznsg.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gbcceulie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/ghluructu.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/glxzgukgd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gmqqdcxjn.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gxnkqlzko.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gpgnqxmoz.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/glxyevpbn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gigejsagz.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/geivsbkkh.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/ghiylhfhe.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gtwzmygzp.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gwmgtrlph.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gjdptixvs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gukjmktmm.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gidbxlbmp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gzykrdjjv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gwiutwdxi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/grazaokkw.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/grhpllvsv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gjnfgmqnq.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gkqvzqtcz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gubhhdubv.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gmnqjoubf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gfidbvfyb.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/ggkalqvlg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gyizmhcmw.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gsmflfjnv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gbsitfoqh.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gucaekfvt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/ghggbngnz.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gahkjjtnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gtzibkwsz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/girpdrvrp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/gazszmsec.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gvqhftizr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gzbwcgigg.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gsjjtkjyu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gwqdcamjh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gdkgxloqs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/girdaoecm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/gcgfumaaa.sHtML


<!-- 参考信息 -->