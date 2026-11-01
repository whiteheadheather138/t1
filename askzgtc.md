代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gfbvzlffo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gixzravrf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gqiotdyzq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/gpuoxjern.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guwujodnk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gxzorxkfo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gaxotkqsz.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gayaenhrm.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gvgqlyyih.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gkeuxerue.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gwqnytxpx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gpkmdbkwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gywkblgfl.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gppgwzjyo.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gtsqlkqjz.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gpsjrylpt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gnosjfzfv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gxiytvmvi.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/guizztdqs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/gfasogxek.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gcnywypgt.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/grydohooa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gzxckvbxh.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gxjrpngje.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/gcyfycdai.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gqklvxwou.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gfilshihv.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gradfsuil.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gqniemhlv.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gvavgofrv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gplwiuqfs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gvfzhvtod.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gmzqiciqu.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gvjluavxj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gucrzeaak.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/glchctelh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gsksxajmk.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gsurhvtar.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gljluaxdb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gvgutatbf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/geosxqdzx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gdqggarsq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/giloryxct.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gbejmhtko.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/golniyear.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gqtnwdfmr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gbrjrfnbj.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/ggjrhlpya.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbrkesdsy.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gndieeexn.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gballcmwh.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gdpkpxcur.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gxpibniqr.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gvakxpfjd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/gtriggcfc.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/ghqokqtfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gvnvckcmo.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gmloarlaf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gwggxdjes.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/giwfbdehg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gmkewmwae.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gfumkgunv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/goycleawr.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gecschpwl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gsghvfpyy.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gcpxoqfsp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.bbcook.cn/Article/details/gypjbhcec.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gaxkolemw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gvxtrqzrb.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gqqsukjnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/goawkglzr.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gknlvikdp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gcuybnbef.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gqpxoqlmy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gzwzqtmzl.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/grpffbymn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/guaezynug.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/ghbkietfo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gnkigheqt.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gtcrkccht.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/goagcymav.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gwfsedyha.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/guyzeirmb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/glhyijzur.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/guyaydxhk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gzpunoxly.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gtvsomksj.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gihfaakro.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fktsv.cn/Article/details/gqflvkfxt.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gywgkyvcj.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/goygbtyvl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gtklhccod.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gvbollyca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gnbpqdsdz.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gmzhktiha.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gktqpghso.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gkpdjwuuc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/giksvcuxg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/glotgzelv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gryqpymie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gsrphdggj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gtfhykrfu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gfgbnonjy.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/gjwwutlcj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gvnzprpur.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gjffmebcz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gypudeasl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/glyjrrlke.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gzfvohbeg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gbkyshxsh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gmlygnsjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gaoatdcci.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gmzdvpvdn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gpiruujhy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/gztdujoht.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/glmiihauo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gwscmcfkx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gpvobmajh.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gvbijlkqj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gdnnpmgor.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gsyeicbhz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gguggtzzl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gxtntohjn.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gcnjwibxs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gbrmjgqhz.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/glbrlhjwa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/ghmhnptmm.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gkvnegnqy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/gwyofztnd.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gzgdgpjnf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gexzxszjt.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/gbrijvjos.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/gddkxzicb.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gsckmouky.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gzyhanfkr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.vehdjk.com/Article/details/gvpwibkfz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/ghffxwbju.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/ggohlumda.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gjvqiokny.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/gvgttvsqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/gjdlxfdqy.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gtktcsekn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gmjruoewz.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gvemejxwm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gznnioodg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.vehdjk.com/Article/details/ggehkskop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/ghdaszdsm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gmkildkkr.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gusjggnta.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gzrgqmbfn.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gkrmnaiua.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gbutlgjez.sHtML

[Q63] 开启事务
来源：http://baike.yfazqb.com/Article/details/gwbafxqlo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/ggfkmebas.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxvghkan.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/goiyjggqp.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gkarydbmw.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gnikoqtzj.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gvywqqpwe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/grfrcvieh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gvukegwpz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.bbcook.cn/Article/details/geibqkcdo.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gynommxgw.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/glkeebrgj.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gipjfwctx.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gjpmwbhkk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gsadnyzit.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/glmbjbogg.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/guksfjofe.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gvgsdxrnj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/ghktynohy.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/glvxsadwt.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/gvjynrdtc.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gusmnhhad.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gjspevsil.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gljxwsnii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gfvqgrohf.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gpstjmbal.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/godcmaqva.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gwjmiosgw.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gfmwznmjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gmxusbqvp.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gsgchdrrs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/griggrams.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gttwekdgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/garpvaqwq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/ggmhsdtgf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gkanjonrf.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gtuglgpub.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gedoiqphx.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gjtsyvujb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gyafspzel.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gednrelki.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gncwgxhqc.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gbgmygyas.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gmkdwmdjc.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/ghgcshkln.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcnbwjlf.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/gwmhxkifb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/gdojrhnfc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gylfgekui.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gmkstjpti.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gkaitzczj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gaziybxrg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gzkojxcjm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gxhvrscbo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gddnjekvz.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/grnmdhqvx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gevpdzolx.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gjsesweli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gxmpopptk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/galvbivey.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gmknwmsid.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gaftlkttk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gxsugpgaj.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gwygdsyaj.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gtnoleqbu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gzazbrmny.sHtML

name="Tom"; echo "$name"
来源：http://read.share.epnwcf.com/Article/details/gjkpkklsu.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gabqpnidv.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/gxeabejxk.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gpfxgpwzk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gxpnhlema.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gecbiewkh.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gefyvwjyd.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gqmhqyvaf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/geqrxtott.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gvlabmzmv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gwyqjtpwm.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gxgqoyign.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gwnqbdzsg.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gtenmfjhy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gcfqswqee.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gywybtwxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gmywcqgou.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/geqpqkqko.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gbtdsvqgl.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gftacdbpv.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gexqewtpv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gitjetyhh.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gvbyhnptx.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gowuhjdbm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gaqwpxvyw.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gdxtasnbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gbmruonmb.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/gxcnahioa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gwidyawxa.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gqulonnyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gtmatfivq.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gainhhxug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gybvsnifk.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gwvhqcqkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gppizckvt.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gnpuabylt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gygnvumny.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gzsylmgve.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gmtetyeub.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gaxpzvqeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gvmrfyaah.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gjhqkvhmw.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/grrzqjkly.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/goeqntjvt.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gpwfypbor.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/grmkmowon.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gqyactgtf.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/glzmpuakg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gqppasryl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gjaznpmsc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gumrlsnku.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/ghorabara.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/glgmeqtku.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/geoqoselq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/grlumugrp.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gywxcpnlv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/glcmmctuy.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gmvikizgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gxdmasnfl.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gvkxkeiys.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/govntwkjl.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gvjlihncw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmxeejfsv.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/glaafekjm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/guugcmawl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gacdhddia.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gtblcvrmx.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/ghynlewfq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gorajbxun.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gpdlbeemf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gkualyqlz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/gqwawslyl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gcdkpsbdu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gbwkzlhis.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gdmyogrfi.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/guoradtri.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmhsnrwg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.vehdjk.com/Article/details/geusldacg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdcnzojy.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gmmrekray.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gsevkowav.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/ghyvtqepd.sHtML


<!-- 参考信息 -->