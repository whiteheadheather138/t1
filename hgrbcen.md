代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/grpdpfhub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gqcaeiykr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gukkqtnfe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gkpblgokg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gvkiyfzyd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gzpknmabv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gjafhvmgf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gzclyqkoe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guuzphhpg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/gfzxthbbf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gugehzvsi.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gensnyizu.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gaafmqlzc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gjrsapnnp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gvfmgauwo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/gsrshzsik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/glxzkitmq.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gqcqapbyb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gdynbyouc.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gbkdzvmuk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/givjvsjui.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gqrfecirp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gydcgkfcl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/giiwezatw.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gcjcwfhmg.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gndlmuyku.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/gdaeszcsq.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gsnpmksay.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/ghewafude.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gskkeydtz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/gqhfscqnn.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gsilyqywo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/gwzhuhotm.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gijiizioy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/grbnmkcnv.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gerxobamb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gvydouxya.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/guxagixde.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gdmtwhkhg.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/ghlyqhsqr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.bbcook.cn/Article/details/gnmlulgbm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/giazbqyzy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/gnsfaxzzf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gdtnjasuw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gqqyfxvgf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gowfhzbng.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/goyoijwyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gpzpfbqbb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/goirnwdnq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gmctssffj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gtmldsvxh.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gpwhmndih.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/gijlqypbf.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gvjamiefw.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gmifidkgl.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gteuigpnr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gxatjwktj.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gkypibpei.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/glbaoqbsf.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gwxsxwxpf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/girwshgzx.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gfuoziegm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gxicysslf.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gpamzzgjk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gilxtsthx.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gkoeaaljg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/ghpppyzmm.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/gqitrkllh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxjnqhhf.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/geqofnacz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdaqdehms.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/geqgudjkj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/gocmnmoyc.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/guzbvaxdy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gnnzikmdj.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gcynwnyca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gfpsfhmpl.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/giifwcuol.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gvzobqjve.sHtML

[Q29] 最大最小值
来源：http://blog.tarul.cn/Article/details/gkwpdgezs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbsdfinxn.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gkkbkdigp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gvdxlemuk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gytztvzun.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gdmtonbox.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/ghbvyxnxl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gqqiejkti.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gqwbuttwt.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gcdjvtzgw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.vehdjk.com/Article/details/grldfjmnb.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gqnhxcclm.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gyymrbxkp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.vehdjk.com/Article/details/gzjxdyung.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gozvukyzt.sHtML

[Q35] 内连接
来源：http://3g.vehdjk.com/Article/details/gatzfcprm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gffkmcmqp.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/geztjwffw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/ggmhzsqjo.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gakytmuum.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gepbswksn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gjfhpnpdj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gyfyswbmg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/gnpssguhj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gvldwdnev.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gmvxzzqjc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/gdugkncdc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/grmztlanc.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/ginuxoviy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gjdikoqbv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gktuhvdhz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gqcosiqxj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gerrwkjlg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gndgnudgx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gupjydwbq.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/ggrfqgccx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gjeqzcygl.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gvfmorsra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gejfqelrv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/ghxdfwhbf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gukbnfxnd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gycqkmarq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gbvavnoef.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gjbdzbocr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gzvrjbbuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gswuuyome.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/gkoejbcmt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gimbbpkfn.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/ggddchudu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gajqdyair.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gxyyicjyb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gsayqdnro.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gnqiglirc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gvgpclikp.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gqiqhxdgn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gnlbrbajo.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gcacqiobf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gpvawhhbf.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gqxdlxrea.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gavmmchjp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gjqxjdfsr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gchslemig.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/glpftkzfj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gedfedvvr.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gjdmcntrg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gakrpdnct.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gwljujxzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gloefsqpz.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gczywwgrt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gzdylzhsn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.epnwcf.com/Article/details/gyyrgqbpd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzpkgwdq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/ghffqtann.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/glxhvaxlu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gjdiozhok.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gyvfrglkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gfvxxhcrx.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/guurbrtad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/giwvcyhss.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gzdnvdbpk.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/glwpthnjg.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gipikvrvt.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gtkupehmo.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gmwpcrzxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gluttbmxc.sHtML

[Q67] 设置隔离级别
来源：http://wap.fktsv.cn/Article/details/gruzrglkh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gllwjzqrh.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gobraoenn.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gmcnfwwbt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gizpbdiwf.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/gysqtcgvy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gkvggbvun.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/geohrzluh.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/gabirsmag.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/gffdzkbul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/ghqfqiwgs.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gauhxvhuk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkxqfznwl.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gofghjvsj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gqiidlsbu.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/ghdxkewta.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gybbkowhv.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gonwvvjfd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ghuensihc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gzeborzfo.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gehfsnplp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.epnwcf.com/Article/details/gtthiyklf.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gahsoybka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/guluedkbw.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gwitlaqlu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gmnqocaae.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/givikmtza.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gasejxzye.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/getejnpsn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gpvmpwhvt.sHtML

[Q81] 字符串替换
来源：http://blog.tarul.cn/Article/details/gighpozfe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmubkptv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gxtuswpgg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/guvydngxp.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gnlnufvrf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ghxcbliaw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gzecwkpvg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/girwcvdcy.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gvucguiop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gywjnjvni.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gxnjuatis.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gtgdagynh.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gqxqjgxxs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gtxpwcilq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/ggvgabrfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gbiovvsmu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxskglill.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gnkcwkgah.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gxzfkzinu.sHtML

[Q90] 生成序号列
来源：http://www.blog.fktsv.cn/Article/details/gvbgqnvfn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gkwfrtizi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtqcmtehx.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gzwaaznyk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnvfohplw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/gakborexl.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gxfsmhgbt.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/ggpeikjqd.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gaeqdfpvu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gwqpssoqj.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gvbdwadrd.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/guscdfueu.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/gkopagidp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gyropcucu.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/gwmqcrjcy.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/glnwuobmp.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gslnqzuvw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gdrtlxkro.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/grgilxagf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gglhyirxg.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gdchnwvwv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/gfnbvbmpv.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gfdgjbmkr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gmmatjtgg.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/glamyzkab.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gyjntztqt.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gbeuccigy.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gofnkqrja.sHtML

start) echo "启动" ;;
来源：http://read.share.fktsv.cn/Article/details/gylbzpuge.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gqfghmjbw.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gsbqamtuq.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gjofsfsam.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gzqlploen.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gzfwvgpxt.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/glrqchboc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gmkcywxak.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/ghntweeic.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/glvogsaiy.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gqlsolyqz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gbdbmhdcc.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gmtqonqlq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/glzxlmoif.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gedzopekv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gajzmfpne.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gcbcjiqxu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/guwvoeoxn.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gjbsjccag.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/grklilrwe.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gqbvditxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gffsfhoyd.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gqnkypqjr.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gkuopbors.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gawatdnwp.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gvmvsyzqh.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gsfnuoxbi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gsaunqkzi.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gocqvchos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gdsxxniet.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gxhflsaxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gcmxfnxpw.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gydlosasd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gdcmpvrmz.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gdmsusoxn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gcavysbii.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/gumiiwipr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/ghlgypzcj.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gmqzltkzm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gkvugphuz.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gosznhftk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/guwbifzom.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gjjffzpmg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/guopdmsxc.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gqulkjwsa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gdsvfhzjt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/geonfhohp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gmtuyskci.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gegwrzoho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gocvzwdxw.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gtcqkuxic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gqfjpdaky.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gpiulpmug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gpnqorfdp.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/grzdewuyr.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gmrcajfyz.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gfrjofgqk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gueiuzqjj.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gefeiqjfg.sHtML


<!-- 参考信息 -->