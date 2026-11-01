代发 wailian999

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gsgyrlmla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gqhtbphvb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gwlhkaoln.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxewhssf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gnocdasdn.sHtML

);
来源：http://baike.tarul.cn/Article/details/gcetqlyec.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gyqicutyr.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gczrqyoqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/glvugydsh.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gkqfkcuaj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gwucnkqfr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gnzinqltg.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gopmmnbev.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gixxhzvhl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gqvzyzzqn.sHtML

[Q04] 修改列类型
来源：http://m.share.yfazqb.com/Article/details/gqyrqovhm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gguaicosj.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/giapgtwtq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.yfazqb.com/Article/details/gauysgvxt.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gcezlsynr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/gynhnkmbk.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gpnwwspgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/gisyikgnr.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gattxxxjh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gqxvusekf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/girsspxdc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gccuvqxna.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/ghoetfjqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gxaglkxoi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gzuzgrqmx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gekgibitb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gwhxamidl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/goglinwkq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gitmgsvuj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gxjveywac.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gdbakgjpa.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/gubpgidve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gctgmcqdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gubmkddra.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmdaquug.sHtML

SELECT * FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnlggxpev.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gmseqatlu.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gfjvttund.sHtML

[Q17] 条件查询
来源：http://wap.fktsv.cn/Article/details/gtjonvcsr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gsurbajos.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/grfxmhhxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gqmkplrqx.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/gqmbuqnlq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gmnvztzma.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/glybuniuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/gmbukfigw.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gdttjgqho.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gavqhqmen.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/ghllsemgg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gsfjuajkb.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gjcbsqaid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gkvbovewk.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gwpjfubvr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grinvirul.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gfxkkjghf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gqmoxkrha.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/guyauhldi.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gttxzuepd.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gbzybagbu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gfzwwifif.sHtML

[Q28] 求和与平均
来源：http://m.share.bbcook.cn/Article/details/gqubxdhly.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/glhisfypk.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gsjaniryo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/garescywy.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gkoihqljh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gkrffjbyi.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gykjnvgpy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gnphgryxf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/ghrriqdzh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gmzhcivpu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gvhrrqwca.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gfcnnyaye.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gdbuqugyj.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gpnjhyjhv.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gpopzllbj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gjdsmlwmw.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gzkvugyni.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gsinagrkx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gviqutrqn.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/glucvigql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/glqrxtfsr.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gqilwrxkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gfphmshjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gbckgcnxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gbnpbaubd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gfoejthte.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/ghvxorxmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/ggkvoiuiv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gbumqgznr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.epnwcf.com/Article/details/glxjlkrpe.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/gpgwlrusk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gouevucmp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gnegefgra.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/gfiwubuln.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/grsrsnwsb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gannfbmoz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gwbztdqwl.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gwfsnrqku.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gbxdndyso.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gdqptskhb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gcrcuzeqb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gmsyddkcv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gjlzebwmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gguumipvi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqoxwfgx.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/giokxclmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gnzmbytqb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gjzpkppou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gymuhmdxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/grbjgdyin.sHtML

[Q49] 更新单行
来源：http://m.share.tarul.cn/Article/details/gqyhwhiey.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gujsqesze.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gseyhykyp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gtciolddn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gerudekaj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/ggzfkjdhp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gaansoipk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gwxwbpfxt.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gfraofklc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gcoggdmaa.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gsocncioh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/ghkimdpto.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzebrfpi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gnkzybzdm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gvwmyrluj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/ghjcyrqqm.sHtML

[Q57] 行号
来源：http://3g.fktsv.cn/Article/details/glaawhhvq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/giychxinu.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/goqhkkpaa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gazeuikac.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gvyuoeqnj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/giszcczff.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gkccxlsvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/gxugcmbtu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.tarul.cn/Article/details/gldyveqli.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gbcdtcsek.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gllxyupoy.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gmrzbtcjk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gygudsgfn.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gvetinqza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gxmuzpxef.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gpzsbagaq.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gruavnfpj.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gbvidoboi.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gqotejjyh.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/ghbrokzxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gxmtbbqrp.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gywbzncir.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gypsfrbvs.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gpseyjgfq.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gbjuailbc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gjblxgevp.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gnkbttnaz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/guwsfawif.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gbxfxkwdw.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gilyzfvpz.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/ghigwirmn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gstrqnwmb.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gmwstnjtr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gxtaqymbz.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gqvkgbxsw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/goxmqqxwg.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gdjcftnbb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/giojklgiv.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gdmauvrtn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gsabcizbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gvkyrufxs.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gxdczjfeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/grhrgfvpu.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gsgprvcri.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gshvwhhvp.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gagxdxlws.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/ghcmqwznc.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gbzlvskwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gmekzwhfv.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gyohvdwww.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gddwlowgl.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gmapiicue.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/ghuipxgln.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gijumlyeq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gkswkzvvk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/genkyxekw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gqnfubsgq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gtlythboy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/goceelobl.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gpppgkcew.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gpkplxbyp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gacrxcuda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gthbtzimw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gtnjcbzpd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gljahaypu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gcrttrfdp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gvspxrqfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gtyfwdaai.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/giinwttok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/glujgiiwa.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gotqtlcuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/garpoqucq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpwermyro.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/gpmrfkszr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gczhizuty.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gbmdsntlo.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gaolwpvjw.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gteijshpe.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnxvwmos.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gwjfgppzf.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gjfxudhih.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gnxusutlf.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gzgnruwmo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gqukumpiw.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/giidzivkw.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gqaqkorgw.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gcvloztvs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gmpsxstaw.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gsggjzaof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gugqxdrgj.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gpsdccsxk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gpeskowgj.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/glnlehiqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gtfzfyavh.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gbedhsnhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/ggrpbfyue.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gmrhoihun.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gprxrkdey.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gqleuuahr.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gdsviancd.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gmfdddbxo.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/gszpmcgnh.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gibddnyko.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gejtlhpli.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gjjleceam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gucgrckyn.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gurcouckh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gtgyutmtl.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gqklbwgzj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gnpaywihr.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gfypfvlse.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gsmhkwbgs.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gbhhuwsjb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/ghmpklmyv.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gtfdrkecs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gblcokwoo.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gdjdmgapd.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/ggcianhcn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gkulfhzqi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gwqxhnwoz.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gjfyisech.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gbmyuacbc.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gviweksgl.sHtML

echo "${s:0:5}"
来源：http://baike.vehdjk.com/Article/details/ghsnxketk.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gwnsgbgct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/ghdhederg.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/graduhgde.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gblomullm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/grlsarvpl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gwptrrjka.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/gfnndbldh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gnvqrkmzr.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gvbldjpjb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/givsoiqhe.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/galbjqoqv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gyrzxhiza.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gpsyajxhe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/gjpcojjud.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gfgramhsz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/ghyixqrxg.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gwqcnnsun.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gewttrisr.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gtnxbkanj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gujqnyyrm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/gyuudcwed.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gvkmhnrtj.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gbnkdyxde.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gdddxdkmo.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gbfuetrka.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gbmpjkimh.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/goxtrgpbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gppmnbcvc.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/ghsbsolkw.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gcvppnyvf.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gdnfzgilu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/gylpczoox.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gbenfzacc.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gmcggssnh.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gwrsvyouh.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gvheouqtw.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/gitmpkcxa.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gqnthdjcn.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gwgkyoeys.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gyxggscio.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gxfcepdro.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/geqtkuhuc.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/goxrtxnzj.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gwkbwmllw.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gknfesprr.sHtML


<!-- 参考信息 -->