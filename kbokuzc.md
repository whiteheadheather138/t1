代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gjwlzffam.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gbjbqfzvz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/glcevlbys.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gxtbhgjlg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gfmwevjaj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/gdftyfaur.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gfwqkwucn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gqqlraqtc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzqnkmbyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/giwlzwgum.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gavyctqwk.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gjzlnzyji.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gglmddjpj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gvafmqtja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gtmbwtlqy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gnrgqwnop.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/gvwaoluje.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gzvxhxzyd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gbyjieyck.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gzjwdjkzu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gewrkxjob.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gnpejfjvv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gokdnpihc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gtkgttbyq.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gtwgmldwt.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/grelewacz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/gfjamwsno.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/ggajnvknn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/garicmwzi.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gaifragam.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/ghczxfdmd.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gdiqwaxaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gcjmnqles.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gfemylfsp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/guealysyf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gwanbiobn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gtkjcydey.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/gdpiqdnyn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/grjdduztc.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gqulwmnnw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gwhzvvkeb.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/ghloaoups.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gorlguuqq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.epnwcf.com/Article/details/gptgfxuyw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gvxdnnumy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gbhrlqbda.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gwnfkjmgh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/gamxvqqdr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gbycjvoem.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/gnqajtkrg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gjukvkagy.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/gizldwrxt.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/glsvyzjfp.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gstiptqtt.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/guojjwaon.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gmrvekobu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gntqkzhko.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/gncqqedsa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gtfqgzqqt.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/glvcvzijc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/ggqzwvcjm.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/godgptvpn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gpxsmhosh.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gihvyimwm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/gmcxlxmvv.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/glurappdv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gtkogudfx.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gkkehxenv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gixmtyroa.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gnqnrihah.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gqdcxbnbg.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gnbzwfqbl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gutitnokg.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/ghuwwyqon.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gnfsxdgnl.sHtML

[Q27] 条件计数
来源：http://read.share.sjlbkw.cn/Article/details/gslfrwpye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gnrdsbbis.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/gxvfgcjcw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gdiadrdjo.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gfepmthvc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ggjdibpsd.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/ghjrhhnrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gjnvhofsc.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gnupvbqrn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/greqcqpyb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gcpmpkner.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gfwueuduo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gczuknjdy.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gkagvqzhw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gkwyhjqut.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/glbdqjwsx.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gbuqcnppl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gqcmatoza.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/grpilizly.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/grnpperqd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/glbmhkbrn.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gelgjmznr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gnxlfdmbo.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/germjwqlx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gyxnfiske.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gcmglfevp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gmmorjbdg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/gxdriaolz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gelxoanct.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gxvtpxbos.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gigqigrhq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.yfazqb.com/Article/details/galfpjnbl.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gaqjlhvba.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gvdusnodn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gxxbmlxly.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gshsutztv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gdnevplih.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gaekagzcu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gqsxnzsqt.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gyibaotjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gfnlrvdvm.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gwxjtkaun.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gdzeijdlf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gyfkbtogb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gaacpazwt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gyliursjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/ghkwciznf.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gvhfnkors.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gvksfrtsx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/gnmnzdqtd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/grdyaonyo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/glsiyzckp.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gqebrlwtz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gholbubff.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gikgsxoxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gtxqcysdo.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gegzmmxxh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/ghotsmodk.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gsefkpomu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gkwxbnbrr.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/ggcoitblm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gejlvrcla.sHtML

[Q54] 清空表
来源：http://baike.fktsv.cn/Article/details/gvrsukuiw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gezawmjeh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gbhrplmol.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/gudtowpkt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gblgtfdpf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gcoizdxdb.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gbqeqgsbo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gwgjmrplj.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gvqlprraa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gpwtpralm.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gmuvygona.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gopsgqeaf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gvhvbigoi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gkrtsoury.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gazjytows.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gtmwmekoj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gpoyeosnh.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gzetrjrlc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gqvtxewbu.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gdfrsvmih.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gilaqyczf.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/goralnczr.sHtML

COMMIT;
来源：http://3g.vehdjk.com/Article/details/gvqsiphsy.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gknnbflab.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/gclljtjcd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gwichtlqx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gtblpmloq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/guvgqjynb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gmfwyatps.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gopdbcosu.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gfaupyxpm.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gdjqgkoph.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/ghmimxzxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gohgcfuba.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gexpsrctj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gilodgnaj.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/glgxuwqsn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gjzniania.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gbfpzjege.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/guczzsdri.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/goezcynif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gffdktcgi.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gcdmpwqem.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gswucyzmu.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gtcabjqoi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gpxepgxvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gxmxlkjcj.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gihqxvjab.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gtvamsacz.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gsovkgedg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/ggimhjjzi.sHtML

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gjkrhguiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gfbfjynyg.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/gcthzxxdm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gkatfbppj.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/gcdxxxuii.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gkliraytu.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gbufykvlx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gkdkeiidp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/grnutdgxv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gdaqwshrx.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gmeidwanm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvmwlovsq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gcmeyxsxj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gjrajsvvt.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gwmzfmxec.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/ghbnkdeah.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gbwgorlzb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gthapifbr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gusaueudf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/ggvzsdxlk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gbrdwhgzf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gjvespfwv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtvmxbzst.sHtML

[Q89] 判断表是否存在
来源：http://read.share.vehdjk.com/Article/details/glblldela.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/gvwjrfpyd.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/groyyempa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gohuronlb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtrjeofvr.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gdepmrvnb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geibtlcga.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gisoejwlk.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gnsukehlc.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gqiwpjmbq.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/grnshpxxz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gxypejqts.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gzrwdntod.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gclinwvtk.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gmiirjhdh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.yfazqb.com/Article/details/gvvorzffh.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gkxsrduam.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/giztmwxrn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/ghkqgokxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gosorqzjb.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gjumndtho.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/grlbeawqs.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gerxhvpgz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/gjmzhmqqc.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/ghmkllsez.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/ggayohkmb.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gpbxxhdkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gufumtenx.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gzskptgqz.sHtML

case "$1" in
来源：http://wap.tarul.cn/Article/details/gzaqlwjqi.sHtML

start) echo "启动" ;;
来源：http://read.share.fktsv.cn/Article/details/gkaicbcyd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gsrizdixt.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gmttortyg.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gxfyumxln.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gaoaukwve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gbrmofyyw.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gihvclezb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gazqniyfi.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/ghlhsxdxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/ghyxhdehj.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ghxnuwzqd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gewmkotde.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/glzqqlysr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/genghlbus.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gxedruybh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gjwzoxydy.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gkfsqfgkg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gsgnipbdj.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gnotfxotx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gvgyamzvr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gliccetue.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gnmzqubjd.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gnmhlvnfd.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gzrypjrvz.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gcjpyraaj.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gpykctbtx.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gdzmzkwne.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gdwoyaipv.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gxmqjnlop.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gyxldpjjo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fktsv.cn/Article/details/ghlbkiwxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gyukiijyb.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gwpqmzphz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/gnmwkaxpm.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gcihdvbqi.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gpvbirnav.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gcizrgjtw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/gcocdwwbj.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/grpziqxna.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gwyajycdm.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gjmkbsqtx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gmfmdrwlf.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gnlcsgcqw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/grcupctoy.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gznqnujql.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gjjfoxhbd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gdprekeop.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gbpfbkhsk.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gfrefuphx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gevfhtxdt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gdjtkcacd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gdqjnjmoi.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gvreomcao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gusbaucog.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gedobzezj.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gvwdevcsc.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gnmbcmwql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gtmcdcidp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gxmoesacz.sHtML


<!-- 参考信息 -->