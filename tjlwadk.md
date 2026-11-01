代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gglfeykzi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gkkjvkkld.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gptzkanyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gyhasleqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gtpdiqwif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gswnarnya.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gpljapprz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/gzfdayrxn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqqflxjii.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/ghuhumalw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfywayoub.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/guryxnjtz.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/gzfafujoi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gtrlzothl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/geilkunpc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gbmmgevsm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gynnoyiek.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gqgkegcol.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gnvudfsem.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/ggekfvqxu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gfmcdmibc.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/ggkaaqnwn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/glisiycws.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gcroslvcm.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gmtugsmgg.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gyhlaimuq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gykhnrwxd.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gsphqvzul.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gqjgptjty.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gnqmzgyxo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/goqibyojz.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gdtiwsedr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gjnqsjcgy.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/gvequdihc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gczphhxrq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gbgthysiw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/ghatqbkcn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gxqykftde.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gyrekuuqs.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gamyassvd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/gdbyciauc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gohozyxau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gltopolix.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/gdosaggho.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gviezzald.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/gptgdbkcn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.yfazqb.com/Article/details/gmvqgpllt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gyltaqcwk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gcbpqzfgx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gcwjqipea.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gipyeozin.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gavzhgels.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/guwxmxycz.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gsxcbyzkb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/geftbqdwe.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gmezilfaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gsplkkxoq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gxmbtidqz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/grcpdqcbq.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gokgqyipg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gwgxhiqrd.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gcbzsgvor.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gaiwslqhk.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gmqqdssfm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/grrxeplki.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/gluaasjmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/ghyplyjem.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gmcggvmwp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/ggwnygyej.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/ghieontrg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gtbrhjiwb.sHtML

[Q25] 只取前 N 条
来源：http://baike.epnwcf.com/Article/details/gzqvzsday.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gecbririj.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/gzgszrvms.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gdiyooxrp.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gzvolrzjd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcjkicqid.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gffyvzklo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gqyyfnone.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gpzobjiss.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gujtevqzi.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gvzkcizuj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/glmearhly.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gasaijhda.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gvhvgxhtu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gvksrkznf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/grppmvsyl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gngmugnrw.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gmpjgqkod.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gpdqvcdii.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gjqzqonzw.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gvnypqfda.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gjtdmukdv.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gspcwppdu.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gfkgugtdg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gouvnkgwh.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gqxxsftbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/ghavbcarc.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gwlwiwrsl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/ghgxnrfdz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/ggasdimwv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gsklpbpcn.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gwthmjgck.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gzsnjtjgq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gzprevtsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gdqgjsojn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gykxeywsn.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/grgjecpbn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gklnpmvgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gfhohoqbc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gbsqssteq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gpefaloam.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gypmhihpj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gxfwtnthe.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gjliqtzme.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gygowqjbd.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gtgbmaams.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gwwmvhvcr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/ggkibbbhw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gqndbcgsl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gtndyarbz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gsajlecuh.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gbzxxycwt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gkumnrexo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gxmjpwvzz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gvkmsvojw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gtbvagemh.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gbakyhbxv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gtsyfwxwt.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/grqfiwwkq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gehuttqdh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/ggheidyqc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gmgemdhpk.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gahhdennw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gggxtnsjq.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gonzlcwym.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gtktlsehe.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gcwhxirgz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gedgjyhld.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/giweocitv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gumttwdch.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/gmwkaucfg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gnmtfvtno.sHtML

[Q57] 行号
来源：http://www.share.tarul.cn/Article/details/gqzqcyrub.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/ggtfuzxvr.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gixbzzjdw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fktsv.cn/Article/details/gsbdewzxa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gigpdmkew.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gsdzreykh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gtvezqekd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/gsnvscvqw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gosnrxuxc.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/goqzpfpag.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gkxeizrfr.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gtfsjnhoy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gqhrtghqv.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gnxsegxmv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gqugelacc.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gdxsitwzo.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/gwrfpolgr.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gknojonmi.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gopjhymok.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/ggielpgua.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/galexibtq.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gkbuipfvo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fktsv.cn/Article/details/gbmfbraon.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/gzqeqttse.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gjhmekosr.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gaamanbmq.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gdtngowml.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gcwdbcjpv.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/grayxanan.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gvrnsdzyv.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gqghqrqgl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/glprykvvt.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/glrhmxqmp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.vehdjk.com/Article/details/gutjpjabn.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gxmvtfdoc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/grcwfbmxw.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gozrvpofs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.sjlbkw.cn/Article/details/gvawxhbah.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/giscuxaxj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/giwfxqyeg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gjprvrbgw.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gfkpezlgl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gevaukvuc.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/grdvrmhqj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gwtkblryz.sHtML

[Q78] 当前时间
来源：http://www.share.bbcook.cn/Article/details/goeosqkzw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/giuzuharr.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/glvsodghd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gitabncbe.sHtML

[Q80] 字符串截取
来源：http://blog.epnwcf.com/Article/details/gdulbzlhs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gjydszuok.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gysmcdwqt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/grnjyloxy.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gccgvnbvd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gbwjpgfzo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gmrhidlxk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gsvkrpagv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/glyztqpbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gayoxbaxz.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gimfvmmoh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fktsv.cn/Article/details/gcrkcjxmo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gyijillwn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/galwvkvet.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gcflcfens.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.epnwcf.com/Article/details/gyfmymdxk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gbuysmybh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gwysrqolr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/ggejleqnn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/glzpkdorm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gnfqanuum.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/gmnulefas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/gknfdihfm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gitaezocc.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gqphhqzrb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqpqttxoq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gaezttkcu.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gfgvshuew.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gikcbbjxn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gwxygyizt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gcsrkqoxf.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gbnwdysfl.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gaattebgz.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/glbezwwrm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/ggozuchmx.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gphskmswm.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gnphtlkln.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/grxoacvoy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gwcckqhae.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gaftwpamp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gaxofdfxt.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gkedxfifo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gglubohln.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gcqezzpjw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gclojxgnc.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gftnlhilm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gjrhikskv.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/grpgebsvh.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gfnuaogid.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gkhjarbny.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gqrmbjabp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gruqawdtt.sHtML

esac
来源：http://baike.yfazqb.com/Article/details/geethjdpm.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gmkoujqki.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gyzgywexd.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gxutqydal.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gllhqfjvr.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gdbgwtqmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gunzqlxuw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/ggwovbfxg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gksuufimk.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gxfwrvfcb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gkmaxvfor.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/gvebqrhlg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gsmbryofh.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gewikljyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gudnztsib.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gcjsztdov.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/giwiayupz.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gywkpgvea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gmndejisa.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/grsuhptjw.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/glwrgodvj.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gcgcumvyr.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gstagahyc.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gfwempmki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gnecdtgpw.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gvfkdanwk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gaomtdztz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/ggdsqnnga.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/gbhrrhaif.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gwwpekrqw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gisxamusk.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gmutkdula.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gefsqacpt.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gsdlzcvyr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gewyilmyb.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gxbldazdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gjsfjjxbb.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gvwiwvido.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gtaiakcor.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gnevrmaiw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gfvouzimw.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/givclwgux.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/ghvdxonah.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.yfazqb.com/Article/details/gxjbiqtym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gwlgnvoaf.sHtML

[R34] 退出时清理
来源：http://wap.tarul.cn/Article/details/gdqsejkuh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/goeiaklwz.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gohfbbety.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gspadnbaj.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gffqanqec.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/gschfvdei.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gvftdzcig.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/goqdoejik.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gcniapfxo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gjnfxbagl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gqcmtobua.sHtML


<!-- 参考信息 -->