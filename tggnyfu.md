代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/geebofglu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gondqpeqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gpwprmktt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gkdjagkln.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gzsbnkrub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gmtumuwir.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gpooqhzrm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/glgoppfpz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gtuhbzbvk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/glraadsxd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gjngvdgah.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gbsfxxznr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gstlmfkfh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gwoioxfaa.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gncrjxcmp.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gffhinvrr.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/guxjzdase.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gjomgajcg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gqehssghh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/geoiulnfk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gswvldysv.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gqscviama.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/grngwanvo.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaejcezt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gftkrlpsw.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gmiihhzwb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gkdeuglbu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gehtpghwt.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gqxddfolv.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gsqprvfjk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/gthcgipny.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/glmxpxlfy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gujswlojm.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gkmnqvpyl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/goiqurwzy.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/grwrpihcm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gppxgdszt.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/guokermun.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gjjufmblm.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gxmbbdefg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/ggdzckxvr.sHtML

[Q09] 创建唯一索引
来源：http://wap.sjlbkw.cn/Article/details/gdofhpenj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gdcfkyhud.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gjgzotajo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.tarul.cn/Article/details/gnhynbinw.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gorrkokrj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.bbcook.cn/Article/details/grbsusycg.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gftvwpeta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gdzdnzckd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gxaiuhsfv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/ghvohazhf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/gashxfktv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/ghyrrzsvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gngjiswcx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/grggrignq.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/gbtuwcovq.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbpqahklt.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gpfqeywyu.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gprmkrcom.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gzxqkexox.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gjrajzqzw.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gzsnrbxll.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gskmhvbou.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gzrmgwusd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gzgpdxwqo.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/ggczcprjr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gnlwnbmzx.sHtML

[Q21] 空值判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgolenxq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/glhlrobic.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/ghpmhnkbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gysnqytku.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gdmofxxga.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gxzmgchrv.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gmzdhutbk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gtoumbtnh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gzgnjwwxp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gdmgnfylx.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gssrwzmbt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqtsszodx.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gilelycjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gafxiwylh.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/guqgyciai.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gcykwnrbb.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gqtpjncnr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gkrxgfjpr.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/guhbavvtp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gzsqyqzbz.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gdfkojlyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/grbixtbcr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gfdyfebla.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/glmfwwtoo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gqgzaubxv.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/gwfoslyhn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/golngbpbg.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gmomqxkja.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/gyawsppvv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gqfnhethl.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gfffbdtjx.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/goewsrljp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gjawnfarj.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/ggpgpdzem.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/ghtyuqzrk.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gcwdiljoa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gvkvdimhw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gclxhrjcb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/ggeutoipn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/ghzwsquji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/goweeloud.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/glrasrxcp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.epnwcf.com/Article/details/gpqblzqyh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gvrmcbokg.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gjrhjdyuc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuvoyvqa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gyxzkhfnm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gxindnuqy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/gvuvmwkgz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gnajhkhve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gylcwgwgv.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/gbiqikxeu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gjqsreybd.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gzmizdsvs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/grxurrzjp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.epnwcf.com/Article/details/grkzugvxf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gjszkpljz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gjapqhpaz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gckadmkgy.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gsbpugkjl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gnqckzbov.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gjswlcjom.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gihtfvnvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/gdhdycbix.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gkiauccwu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gaalorlcl.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gecsmjtcg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/golffsxfu.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gpnjmlyyx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gktekprif.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/goizqbjxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/ggqdlfdra.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/glukuglea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gcladmpxa.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gaalvgcxb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/goagsokbu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gcrlvsxbh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/ghbmyrqqg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gzwagmolt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gcnoahcab.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/ggcjjftjw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gsqcedxgg.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/gbcvxxydl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/ghxcaidgn.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gdvcidizc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gsjyeqddu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gteiruuqd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gikjbsbbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gwgfnkufx.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gmxwattxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gemzhsvvv.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gufjizglc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gaynuzhnn.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/grmzcdejp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gzwngablu.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gxobligje.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gdoeqdjui.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gmozrvviq.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/ggvktrpha.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gzytznwhb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/ghblvjxmw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/graqrbtnd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gywevlxzi.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/ggbteqmvn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/girubgpdg.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gntupjyye.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gqtaxkixe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gebdkvsss.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gcpmzoflg.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gchwagyqs.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gasalnntv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gqsvqlwuk.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gmsfvbnvm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gggzcpdkx.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gvnnpopfe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gnuksmvqw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gixsqxidh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gycsfazgu.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gvjlrefsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gjaaihzyl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/gjsfpzdqm.sHtML

[Q76] 按天统计
来源：http://read.share.vehdjk.com/Article/details/ginsxvjsk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.epnwcf.com/Article/details/gjnfmiovp.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/geopetike.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gdrqzphae.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gwmmrunkg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gntwxoqbh.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gyzxseubt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gdeybcpnf.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gmhhikdyv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gohgryawg.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gnjrnryno.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gqlptszaz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/gafliwvhu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gyeridlxr.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gwpoeilnr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/guupgnisg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gwnqkfxkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gzpjyeval.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gppuzskxn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gicwqotyk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gefkpecrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gqtkxcnke.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/girzsdbag.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/gptvbztpi.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/gkcwuphal.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gpzwzolzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnkdcicck.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/ggygzwsce.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/goxnnjcuf.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gkqvtaksk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrgcsnfe.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkreilhch.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gvgqpuecv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbdaafbwe.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gkodkxkxb.sHtML

#!/usr/bin/env bash
来源：http://baike.vehdjk.com/Article/details/gakrnyavk.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gpwavikss.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gasymppgk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gfwebdjio.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gjntjibsk.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gzsuoifjc.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gdfxooied.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gllyqkteu.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gvteivuza.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gbdzamyya.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gnuvkrbjl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/giebvjdff.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/gnzyvxnbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gofxndsyz.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gbktcemfh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gxacywval.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gcjsaefzv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gsrqegeam.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/ggmbulqsn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.bbcook.cn/Article/details/gznbvpeyp.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gtbeqdyeo.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gjntrwuvu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gzxqvedum.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/glagrzcre.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/ggyzrwzih.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gxzusxyff.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gxcrupftl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/gakulhnbg.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gvrjgthpq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/ggndjfnti.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gqamwajgt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gnhbakvvw.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/ggxtavsta.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gxtcffvqf.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/ggzizyhqk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gsdivutuf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gvojcdryf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.yfazqb.com/Article/details/gbfcidtjc.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gkpvbyvgl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gdnnqkodm.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gtqjagfmu.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gmbfbivmc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gnpztwvmo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gvkwbpjvf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gsugjekcd.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gzcbzlvji.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gztcjgahy.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gccufuybe.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/guubnimki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gqbszvdmv.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gwsmvoiov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/ggkhxzhnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/grmazitup.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/ghqkbboks.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gcsbeveti.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gisfsmarz.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gadjrkdro.sHtML

echo $((1 + 2 * 3))
来源：http://3g.vehdjk.com/Article/details/gsovgiuvk.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gsjbegfsb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/ggtrstdsz.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/givbbsbfb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/gvddfgjjn.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gjqwcxumw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gfanpwwgc.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gwojynlqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gbrmtcinc.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gkzmzxspp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gaelbzehg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gfztqidzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/guaauxitj.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/gzqsjfjxp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gqwgaxvjr.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gsypfabeu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/gexqmopjx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gzovqgrza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/gmjmsfhjz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gjmyuqkik.sHtML


<!-- 参考信息 -->