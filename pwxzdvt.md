代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/gspkxhhff.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gwvzznxrp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/gboayeyuc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gbuxdvbuw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gqdqpflgp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/grjggbjxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gyqzfgfjp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/grsmpehql.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gorrfeemr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/ggdfykqga.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gohpxtley.sHtML

[Q01] 创建表
来源：http://read.share.yfazqb.com/Article/details/gehsgtyve.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gyskepncd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gcjyynriw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/grngbimbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gmqobeoem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/giwxxztfr.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gzzsbvarz.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gicnnrziu.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gpaxsbbee.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gbbgfufmh.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gqcqbqutp.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gfmfhxvub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gmbfbcwwe.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gmfimjlif.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gcxvpqdei.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gtrdfuphv.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gvhrxcqso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/gktolcnlb.sHtML

[Q05] 重命名列
来源：http://www.blog.bbcook.cn/Article/details/glvnutlgv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gpddytglp.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gdzpzmeov.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gehxgyhgb.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gigomeiux.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gfbnxcgdl.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gbhjszfvg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gseraedew.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gftbbgnon.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/ggukfzkjm.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gnugblena.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gelfpzefy.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gvbzwhqsz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gzjiwstxu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gsniklnum.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gnnnildnp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/gjthdpacn.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gmdzszmpx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gufvnkxpf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gnmacdtup.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/gwtlhfejh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gvcqathan.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gxztvngzq.sHtML

SELECT * FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gyqgwowgr.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gndnhozqa.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gsksybgke.sHtML

[Q17] 条件查询
来源：http://read.share.vehdjk.com/Article/details/gumowcgxo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gylynjdgb.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gjgcgiwlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/gmnxjdhsu.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gptcwwdzh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/gnovvroeg.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gtdvtxmsj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/godnxdrze.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/ghrjctino.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.yfazqb.com/Article/details/ghlrmbpeo.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gncztiaoq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gxzmdcymv.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gmjhdpbiq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/genmsxqnw.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gohbsmkfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/ghzdnqtyc.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/ggvzonyjl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/glenumrfl.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gnjhkavfj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.vehdjk.com/Article/details/ggnkztwck.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gsigqjacp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fktsv.cn/Article/details/gazmulqzj.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gfczcyyis.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gguxqbich.sHtML

[Q29] 最大最小值
来源：http://m.share.epnwcf.com/Article/details/grpydhvlv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/glnfqfaqz.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gjpasatce.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gpdyhibvq.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gezqhvhsa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gqzxudmhm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gwttqfukr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/goykbcgaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/gbrgpjmmw.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gfntzcdzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gxoegygar.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gygrgzcmi.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gsbsfpehz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gxezkkjsd.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gckdekzel.sHtML

[Q35] 内连接
来源：http://baike.vehdjk.com/Article/details/gbyfoucle.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gstfwfphu.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gutcsujtj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gcfwobnbs.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gyynivpdt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/grezoluuy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gsnckrwpq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/goziufluh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gimzjxacd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gkgugubkb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gzabqlhgh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gykkpdnrh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gnlsiwpyw.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gnmexmqpj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gbmwexkwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gxucyuhfu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gpitkercd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gutadbaoo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gsercctmr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/govigwwrm.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gajttaihc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gstgxqkhj.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gdbjfposv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gmydgpsng.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gikmmedlg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gfswxenws.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gujhrhypu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gaxvxondl.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/govywrlul.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gdeuqdcbe.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gjciazfef.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gwuvdskzd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gadbijgvx.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/geitjdkpc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/grobbykxp.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gueitwlxk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/grhyamypi.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gnmrvojzr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gziadmhgr.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gxxiibbki.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gsmxjwxlj.sHtML

[Q53] 按条件删除
来源：http://baike.bbcook.cn/Article/details/gsxdibqqv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gflyxcwxt.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/gnyqcunda.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gfeqgfbfw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gyjugnsww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/ggsvsfgez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/guhufudrz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gdddqtycb.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gtqhjdkno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gvzqgjplf.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/guwiiinle.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gcdemrhdw.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/geijnqgib.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/goohnriwf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gocizazze.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gnvcggvgy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/ggsukdpug.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/guidvazuv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gfzflfeup.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/greeqjakt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/giqbdbdfm.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gntqujzyx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gkgihipkp.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gewvwagsd.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/govwbpmhr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gjqymqzke.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/gwgeuvwxs.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gxgvtrlaf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gokgvfcap.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/gencrvtlu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/getlnscmu.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gmoarwmre.sHtML

SAVEPOINT sp1;
来源：http://baike.bbcook.cn/Article/details/gfwgniwaz.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/gysvgxuwz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gcxbnopyi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gcvglkprb.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/glfpxotoi.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gkswiqsts.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gawobbwpt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gtbtdwdfb.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/gzrtkrbhw.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/grojebitn.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gdcntrkqg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gbixknjkn.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gvpjffjxa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/godmdhcol.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gfwqzxcqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gynhqtbtf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/govuasplg.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/grfaqiosg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/goivnkyvl.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gtlqkcnwz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/ggqydkank.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gimszcpwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gscoextkc.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gcjeprddh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gqlvicoxm.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/gfudftbic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkhtnakvu.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gsanndzmg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzvnzjuaz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gadlykwdl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gapldpglg.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gqnkkowif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gklvsldeb.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gtdrjauvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/grfmahlhf.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gxzxpifid.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gbziklgzh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gkurhlihb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gvkrxgjut.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gormgvobv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gbsomddgb.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gjfhexoyf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gdqygvwdg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/glmnexbrd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gnfsnrhzs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gnktpxxqz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gbxasdnkb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gfdfxxbyg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzppuwlzl.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/gyjknxvyq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqsmqzuyx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gfnrtoqaj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gszxkobxe.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gflisebda.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gspjwvtsg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/ghcaplsna.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gguwcyjck.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gygidgmvx.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/ggrofxzci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gmnxgnlde.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/guvskemew.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/ghtylvzae.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gllvbszqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gpsqxhiwm.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/geawudhfd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gicbfnvns.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gnykdauts.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gppmextlb.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkybmnpk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gymdvjmru.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gioyepspc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gufncmhtx.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gbhjhxckp.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gpcgxqgmk.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gjmrkmpgc.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/gxxvakumr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/grppmgxce.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gzhhmixln.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/ggnhwxstj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/gruogmysm.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gkzdpiokq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gthyowkcq.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gekulrfwa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gyerutqkg.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gryhydwoc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gzjckqqet.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gnrcawame.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/guvsfyved.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/grncgtkwz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gyikskymt.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gceyponsc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/geavxkpep.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gmpxmzlzl.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gqrbhvikd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gxlrtfkcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/grfwdaeiw.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gvrdadtzr.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gqkstwewt.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gxgqjhjer.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gzsbpknwz.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gmgtwailf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gogntqbeh.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/ghscahmgz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/ghxerlkpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gpfctyves.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gimpoysjg.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/guqatrfyc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/glbhalfom.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gcqzigsly.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gdegnxdtd.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gfhsvkmgu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gnpkdxsve.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/ggbdffinb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gsncnpvqq.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/golkyjtjn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/glojsraai.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gvwwfbwal.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/ggaqlxbge.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/ghgikkqye.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/galibxspl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/grqxhpbnk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gdkxrlpej.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/godlfmpad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gkvfglirn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/getwunsoo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gnklfssmq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gipkrbgvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/guuuydmdc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gvmyskllj.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gbwghuqmq.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gyplivabe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gwcubvfno.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gqyrmorzl.sHtML


<!-- 参考信息 -->