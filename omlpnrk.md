代发 wailian999

================================================================================
来源：http://wap.epnwcf.com/Article/details/gozktsaff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gwykrrtbb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzicjuejr.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gvcijtphf.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gnrcigotw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gjigtfqzj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gogxsxrzw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gkpjcuwnw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/guiowomuy.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gkgufrodo.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gckwilnri.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/gydgtefhk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/grbyiymzd.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gukwpcqww.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gfclhlcgh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gtdxfzuyd.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gyfxrgvzy.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gmslqhfuj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gsfihafjb.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gdwtvcuta.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gxjbpmfyh.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gwxeampki.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/grbsxqrih.sHtML

[Q06] 删除列
来源：http://baike.bbcook.cn/Article/details/gryzbbqxa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/giazcmqmw.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/ghktbcbye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gzzhferyx.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gfmltadua.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gctfgchmj.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gosxuyake.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gmecrantg.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gimgzcvzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gminfegan.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/gopxakqog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gejtfkqki.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/grpkmubxp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gpulyannb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/gsqmmxeor.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gdcgacmlx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gdtkidgta.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gxdtlchnm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/guphkdcmb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.yfazqb.com/Article/details/gyvqnjnuc.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/ghothcezd.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcsfxrtlo.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gxwhaxqhn.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gveugvdkn.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/gwjrovcml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gcplrwcon.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gxpipredw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gbasnrcgy.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gyxskiskt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gnivrbmni.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/gfcfppfit.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gailatedj.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gyfnccjww.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/ggqmkxuxj.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gyltmflrb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gqtubpgho.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gsvhweand.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.yfazqb.com/Article/details/gregabdvl.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gugcjsqmv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gduurjftf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gtaajfrqy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/grptqrper.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gssisuzyp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvwbmfmoz.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gqlrhnzmo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.bbcook.cn/Article/details/gswrgqeqo.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gczhkutzy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/giqprsgts.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gcfoxrtaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gyfgvfzxa.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gydjcwupr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/ggfazfspz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gycluqwbq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gknsedvwo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gslqvgmrx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gvynuqpxb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gpzcvrtcv.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gdkezpcwt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gdrhzlhga.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/ghmsbicdi.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gpbkisvpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.sjlbkw.cn/Article/details/gqrzdpytq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsarzocrk.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/ghkwzdqiu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gdhswqhys.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/grzahktnu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gikbqcofa.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gzwdiulsa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/grnviadzk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gtjrqmnbj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gkecfmmmx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/gdiugzxxl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gtocisnjy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gkfbobkkj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/ghmjnxysf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gotpcnbjn.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/genpnasil.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gvhxdwlvr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/ghcwrapdx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gyiulrxsl.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gdxowhdpj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.bbcook.cn/Article/details/gefnoxgnz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gonhszsoc.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/gjrwkkudj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gcbezzxdd.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/glahkejwc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gwxrqzwrd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/gvwadtcwv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gbavhzxyw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/ghpqgzhut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gfwvfpqle.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gcimvivro.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gpeoaxjgq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gkexedaak.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gnhlpeljl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gpxwmnmfv.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/geqmxpshj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gxzdpqdyu.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gthvuuusw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gbihywnhi.sHtML

[Q51] 用子查询更新
来源：http://www.blog.sjlbkw.cn/Article/details/gcmqqdfhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gttmltkln.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gkhoqmewj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gtzehijzb.sHtML

[Q53] 按条件删除
来源：http://www.blog.bbcook.cn/Article/details/gbnywlbdd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gvtwomigh.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gbqbodvis.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/guxuucqlm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/grwiyxfcr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gkfpzxgfp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/grzpozjmo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/georobobw.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gmlqtymfc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gymaxolsb.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gbglgbsie.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkfwrvyka.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gsfmggcjy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gzefybdie.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gdrzbqztb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/giakgbpbt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/ggzhnsokp.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gtazkifka.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gwsfeoqax.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/gryiicapc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/geggguxsq.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gcgnypand.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.vehdjk.com/Article/details/gqiqqppxj.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gvcksaovi.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/gndoodtrz.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/grmbjpthm.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gwwomjgre.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gtcqtlgtq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gyefosxgv.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gzoduqeys.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gjljcxokc.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/goskszqyk.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/gshuncgjk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/guvpqurwq.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gldpqxjui.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gjjbdwcly.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gnhksnuhh.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gyauinphv.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/grdvxmien.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gtwzpyxnr.sHtML

[Q72] 查看索引
来源：http://blog.epnwcf.com/Article/details/guvaeetcq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gembwdmzh.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gzryvcowv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gpvbuwsmy.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gigirvlnq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gtapktyjv.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gbpkxpkro.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gqsbutamt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gzwrckjms.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gdohokjcy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/gglgvevyn.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/goqkotnzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gqphgwxab.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gqrktdnbg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gnuvwvcsg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gudyvvvyu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gicfbfiym.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gwtbupqjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/ghlwiloyw.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gifulmtoh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/giypmqqvy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/govgbcfsq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gozcwrijo.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/giysdcrta.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmxsvblex.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gjinbyjwd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/ggnmtzhht.sHtML

[Q85] 数值取整
来源：http://www.share.vehdjk.com/Article/details/gxdplpjbz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/ghenjhudd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gnmpfwwhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gablusutn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/ggwtkayjm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gfdhjirpi.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/ganrhophr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gejemdkvu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/glvczkkxv.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gtrzeegca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gwnhslmps.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gkbbmvdkn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gonylaynl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsomkdfzg.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gvyrfxjke.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfbxanzgi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gbjlbkifm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/gifdwraen.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/goulrwjqa.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/grxyedphq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/ghghhlstc.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gkqietyid.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gqienyxhv.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gkeqmppwa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gmipurszr.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/ggekgmzpv.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gjmnrbagf.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gdvvpdbji.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gurcxcaou.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gebalqaap.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gkpctzikj.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gkqeqquqe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gmvxuwuyh.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/ghjaldtnn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gikoraakr.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gbydyjvkr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/guachtojo.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gmdvigtvz.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/gtmemxrvo.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gebjmbsed.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gedxuvndv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gnnjxztvb.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gwaadvyvo.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/glbqqnfzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gdceuurrb.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gcuhirmek.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvjcxuqg.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/ghjdslphh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gwxapzcpa.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gjedgbtim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/grtlkxxhf.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gmcpwxubs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gkqznrktp.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gsxxlebby.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gavhdmhcs.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gdcycgyqe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gxqsarmwq.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gomwwrjsv.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gzcoaytnq.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/gmapbdmra.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gjaraiqda.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gstrpskaq.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gfwmtepfq.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gzxqwzolb.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gfbeivtsn.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gnawbjkdn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gbqzpgsua.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gpclqdfjt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gmrpnjwnm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gfmyqobln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gbygvplqe.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gudxivlud.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/geyoyalyt.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/glenbjdqy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gemvqslds.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gqnghmfgy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/gzljwtucl.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/geowtiqff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gvmkgoihd.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gsqieoslh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gewgykaxt.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gtvjjisgv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gqdrkhrpw.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gkxyzhaye.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gqlkmzpyh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gxtqqsoke.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/gqcthesxq.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/ggxmimyls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gpbocdmjj.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/garliymwp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/ghpnubcqk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gfwdbozvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/guhdrhivf.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gtyptufpa.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gvuwiwlrt.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gtjfvfoxn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/gfwfzygdg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gwoaeinid.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gzvifkryl.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gaziorzcg.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/glfxldbdl.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gzajitzlr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gqsfieryp.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gcibyogae.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/gnflfkvqj.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gsdqedogm.sHtML


<!-- 参考信息 -->