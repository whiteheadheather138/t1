代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gpmrxgvul.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gbhoqnnqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gmfryyuzn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gforifoee.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gsoamkhpy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gwsrftith.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/githdwgjd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/godqjynze.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gmnvekvsa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfvqngna.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/ggpmdhrny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/ghwjsdxhb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxeerdrfd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gkrznvffs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghvjiruym.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/gzvvodmwl.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gityfpmsy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/giaxlkpwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gtskbecla.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gquabzqze.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gamkayumj.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gfpexwttg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxquowyy.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gffxhcazk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gpkzezqun.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gzwqkthmk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/guceqipew.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gmepejzod.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gheigdjdb.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gmrnyypdn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gntliufal.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gcnprstke.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gsqlszqlc.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gqopmwxns.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/glkjfmlhe.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gkvevalbd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gjxwncczu.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gkfnqenfw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gtjrrdylk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/giacplorl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gtwxxrekq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/gkmjljzez.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gaaheozan.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gudajntpd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.yfazqb.com/Article/details/gfhxobjkp.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gabmvubbv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gfvygbaaj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/gksasihla.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gcbwioubh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/ghuwxlcth.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gmoqtpzng.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gchyafjvx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/gcapvuowv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gifkljrsz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gdytpmbvd.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gfrnpyjyh.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/guwnmcmdt.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gvqcdktcw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gsgudnwgf.sHtML

[Q17] 条件查询
来源：http://www.m.share.vehdjk.com/Article/details/gzqbvoxus.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/ggnhktbeb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gtmnqnqwv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/grtidvzsr.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gtcbtqzty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gnczsboqj.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/gssugwrhs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/giijmscbz.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/ghsqeogjs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gxcnhayom.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gulyfgfed.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gydikcusr.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gfxkqjead.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/glbemaluo.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gqfbbahfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzdexpvdt.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gzedmizjr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gxyoorzab.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gcnwwuoqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gitkmrsin.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gzkmlzybf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gtwghggax.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gtbwdiwul.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gffawevds.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gcnvvkfyb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gxkrcpuib.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/gzhclqyvg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gakcnnlnw.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gyjsfyxqq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/ggizfzqzz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gksqrymuj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gbqenrtqo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/ghennhfvc.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gtnszjqsx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gsmulowko.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/grxtonykt.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gvbhtiblw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/gifwijumd.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/grveqtvlr.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gzivyjmqn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gmaqtdznw.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gyfvevkut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gxskzdrws.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gvienoult.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/geggrwvio.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gjvdslwny.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gebiwqyzb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gtafqexfc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gytxewdcq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gacgpgevd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gjzyjwqef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/ggjntuzjo.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/geqelftsx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gmvjsexxw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gvydydrsq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gmkmghsod.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gxpliunzh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gbgcfubvk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gbznpfyev.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gjniqbpvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/germswihn.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gkcdbxokv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gfiunlxif.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/gdisqplhw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkgwykhc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gmhcbbbsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gzkepsewu.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gcsixukfx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gyggjeqvl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/glifxvwdz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/glytwyisk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/gykvpmzor.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gtdozywps.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gwptkadft.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gkfqgmlot.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gpfslmjww.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/grsuakyhp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gzlbpwtqt.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gntnbmuva.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gxwhpfjkm.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/ggceldafq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gvglblvet.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gpomodxaw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gbzjwstem.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/geusutlhp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/gpxqnglxd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gwgjrjpuk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gzdbpknsu.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gogfiyoom.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gatleqnvw.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gfnuqefqz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gfdoejehg.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gatryranm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gerphyrql.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gxylukzmv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gtwjutryc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/glrkvwsbe.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/gaydhizvn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/goayfjodh.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gxwfhoggc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gwgsplxvd.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gaexutblv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/guiozxqto.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gmngdfzyn.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/ghzqzotuz.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gkcsduvcm.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/ghxdxymsq.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gevgszncq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gcydxlqgj.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gbmidrifu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gowdxpeoa.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gwwmethup.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/gysyojitd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtizajfyc.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gcyuspeqw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gsgjcipjx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/ghdvcjths.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gwskbkout.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/ggdovhlph.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/goctkmwuj.sHtML

[Q72] 查看索引
来源：http://www.share.bbcook.cn/Article/details/gzvmmrsvb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcjbenwoo.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/ghhthhgel.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gjqhjoufh.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gddojzpcc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gwtyiqhwd.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gbhccqtlt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gicdcfrax.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/gumjevkwf.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gbujjddff.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gmcgshhpk.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gjvffbjpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/guqgsnpqa.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gercgfzhm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gbmvnogro.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gtefjwysu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/govpznkci.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gwndzldxg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gzuulmoan.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gijavdstl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gcjpkvlpw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.sjlbkw.cn/Article/details/gypnwzdhs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gjekwfwff.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gaxhtajvs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gytmkqeso.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gwdisaags.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gzbmjpvuh.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gzyecacgw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gwgwvznnx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gnzahkpjv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gmgqybfla.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gcrnltwnv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gwxnmvksr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/grysjhjek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gigbhtxct.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/gnznsxnen.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gigaxzuru.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/geoszgtiy.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gwgejgavj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gkfgrjegr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gohejbfku.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gystqcocn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gccodyzrh.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gxmyeqwqi.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gglfvcrxz.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gkqihsdts.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gybabknms.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gnqwrqpoe.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gvddghope.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkhixzwm.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/glypndupb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gyszixqcx.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gobgahxmk.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/guiwcgrdd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gibguxjbf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gehjgqzcy.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gqrysyirc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gvbyeionk.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gejpqbpym.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/gyxekzzmz.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gzckusuzq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gsiwdtmls.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/guunlendm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/guuivjxwd.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/geaxlzvob.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/glwcxbcbh.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gnwsrgeea.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gzmtxlcvf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gaelposrk.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gkjctimkf.sHtML

[R12] for 遍历文件
来源：http://read.share.epnwcf.com/Article/details/gftpzwnis.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/geoqqgwrr.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gkwjtoeeb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gjsiwwkzr.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/grscbrzko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gdziggtjo.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gjwvjjnaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gmvkcgthh.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/ghqjyxvnz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/ghxfvqyhx.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gegqlqent.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gdswazvkl.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gnnfbpxox.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gmoyzvweo.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gkkxwdyjz.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gcqcbefkp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gnherurxe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gvaaemuvj.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gqmtgbqwf.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/grbaorhgx.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gyhsjxlyr.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gskaonnbr.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gumvjtjcd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gfqhvnaqb.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gespkujrt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gmqwoduwn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gvtzizdyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gszdnghdl.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gorjmsloy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gfltjgonz.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gjmncmhmt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gdomtfkra.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gwemdmnyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/ggipnbibs.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gfzgtgykx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gpkicaxrm.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gahsclutw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gxbxppcjj.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/goqjsahzl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gyqwojgei.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gddpoasxm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpgdcbadc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gaxfhkral.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gmzckdyem.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gmdamxktf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gjeuuxxwx.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gvdbgfnkc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/giexweczk.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/gucojzthf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gfxweqwun.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gluegbjut.sHtML


<!-- 参考信息 -->