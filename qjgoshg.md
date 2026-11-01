代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gkxtiahzg.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gutkiplnw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gapxibsli.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.vehdjk.com/Article/details/godcmrlka.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gthjgmojq.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gegkpvlba.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gbvhjpizn.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gyploaodr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/ggnrjjhbh.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gsjgmtwzb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gsltkiqqz.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gkxlksdpy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gsjfmkfbp.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gaxtcpbgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdwtpdl.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gaygxywtb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/glluciawj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoizbqwh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gfimwhvjx.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gqhlgbnty.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gwejhdzur.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/gzyzypugx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gobsccugk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gwwcoahsd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gydqwwkok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gsqtyollz.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/grwkudrfl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gcbppible.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gmrqkrjyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.sjlbkw.cn/Article/details/gaiwoujmh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gjredsprx.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/gyopdepgo.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gyhcvyaen.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gesixnvne.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gbzhykviv.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gbuyvsuoz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gxtjetrey.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gsqjsriuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gfgsrntze.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/glieqwcir.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/grzoiajms.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/gofvzuxib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gzuualtxe.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gjndlytgi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gpexxuyjo.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gplycbdmv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gzefztedt.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gsvawnjps.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gfywoibat.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gcjebzppw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoonkmyz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gwcjbkahs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gagsqpzpv.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/gbpdirrts.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqytzrzis.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gxgurtzps.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxyoorejf.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gjiefdatp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gpobtratm.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/ggyabbjyj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gufpjjtrg.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/goyeaynoy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gryqlrquf.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gzdifznqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/glhykiwfp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gecwalcdp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gajjiokih.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gtolrsjwv.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gmfnlhrwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gmjxooncg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gmlvckevd.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gukxvdpng.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gzshtxwtq.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gfvwydtqs.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gkzqsjwnt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gaisrrqzu.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gocymfkco.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gjohgpvvy.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gbhxaondf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gcnlzcsfb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/goofbfwcp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gjmnvuvkn.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/glupwkbvu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/gpcmqjfer.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.yfazqb.com/Article/details/gyefwgwca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gdzipktzm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/gxdwyuuwh.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gahpsncdo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/genitahek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gcmjiasxv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gylswsybq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gdymngdwe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gwzxtivek.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gwhomorrr.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/gkzduqrec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gdfkrgfqz.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gbznblhde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gzpnqpicb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/glzlskfol.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gbhfysfct.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gbnmfdbqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gawkxcqgz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gpkftadby.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/gmzeokgki.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gmlgiaphg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gxfxjnjxu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmrfrmiz.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gjpdftuvx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gxhexrkkx.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/gykyqcmzf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gigtkzhhp.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gbqytnsaq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gowxnovlu.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gjngjavjf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gbeigfnrs.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gvwxkiqfe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/glpaoxjws.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gqotsznti.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/ghptmqpwi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gdehbwivo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gbweuoucf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gropoqkoc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gxifocyry.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gjkqmgxzj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtwsvjhvd.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gkymmatau.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gvfvwcnko.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/gmajunjrd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/giimpyyuc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gtswnmfoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/ghxpqfvof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gztopfqjx.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/gkxiwkvpp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghntsrrdw.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gfulqnhww.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gezptxegv.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gmqbjokag.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/guwetswlf.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gzwcjuqag.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gdabuxtmn.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gbebruqai.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gtjbgsuhu.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gpicwydoh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gwtgocrym.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gowmlnega.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gobkfmhht.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/genomcyae.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/gmpazdjge.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/ghfdqqvvt.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/gfnkcyzje.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gmpoiahly.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gsbmlpaci.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/giojgorvb.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gsdwfymkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gppvaibuy.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/gmtuvtucw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjfluswmq.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gumogzxmj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gdklydsfh.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/grevekfjf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gxpbrjqdw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gxjoonbti.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gtecxsxvb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/giyfngcpt.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gbzdddlym.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/grpfwbwxc.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/guorlepnx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gonpvxlor.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/glibalmyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gueheqnkk.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/grudndjfy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gsdkjmhsg.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gbhebnbpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gxblvfpmj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gqcgeshnn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gnufdtzoo.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/ghxudmnfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gpkniqtwb.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gvvqwihmf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gjjjxoxyl.sHtML

[Q84] 去除首尾空格
来源：http://blog.sjlbkw.cn/Article/details/gieiowihu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gkjiwwyux.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/glgufdfvd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gnpwljrts.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gmlzfqkit.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gkvhksdun.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gdmfpdygn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/goebtdexn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gidoisntk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/gaqewveqx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gjoknbbmc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gecraenfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gyyzbjzsl.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/ggiopfueq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gajceemrp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnsfgsqnm.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gzxouiazf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfbojxvwk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/ginainacb.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gvmkbtsgh.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/goujikrnc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlwfzzbb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gwgcwcqhp.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gqnxffqda.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gshqxrxpa.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gsikscoln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gpcajginc.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gnjsxbagz.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gxieidbfg.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gqqfugkcv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gdqhmhqic.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gsevrallg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/giqgwevvv.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gqstijjbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/grnuzsldy.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gdiradqjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gtzlazyit.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gemyaijhn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gidvxbfpb.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gmbvhkryw.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gylykawod.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gajzeurlq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gvcovqdqt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gssyakdyf.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/grvuybrhr.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gvorjddre.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gooffijhd.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gvlrjomwd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gwijdzqhx.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gnefvlgzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gtdqqoyaq.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gfrulympi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gjzdpzooe.sHtML

[R16] until 等待条件
来源：http://baike.sjlbkw.cn/Article/details/gfgcqlonu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gbpdxsizx.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gfhmhaynx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gdxlgvxfp.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gndysnwhg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gjalcukiq.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/ghkpbpilh.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gviogatzw.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/ggjsiyckv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/goyjqayoo.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gvtriqdfy.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gczfqhscl.sHtML

[R22] 截取子串
来源：http://3g.vehdjk.com/Article/details/geyqonrot.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/gstocidfi.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/grpezklef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/glzhnskfc.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gurnfxxjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gbzufcrbm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gjqqrwncg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gntcvccme.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gdkmqgenn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gwiajotjn.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/ggxoobgny.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gkkicrfdt.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gkfaxkfbt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gjkodmafr.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gnnktigjk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gvrnsvols.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/ggjhhyrmv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gfklvfoty.sHtML

[R31] 局部变量
来源：http://baike.vehdjk.com/Article/details/gujayyshe.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/grtgrosqb.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gwbgmsgug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/grnmrhaza.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gxvniujov.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gygckqpao.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gdvbpnfzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gbokoxtbn.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/ggvxlgrgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gotmsygfn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/ghbylnadg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/gwgylsxlq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gprcthono.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gxlzyxsug.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/ggdhtpfmb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gcyjpatqr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gajtrrvhk.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gfldivmnb.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gkrpmjqqb.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gvmbkvvun.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gkvyfqyfm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/ggzzmukdy.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gohfkeris.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gfoqzlqpo.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gkdskfsnq.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gysgvqtmd.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gmjdmpnck.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/ghplgmehz.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gldqvadcd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gglxjynhx.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gljhztewq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gadffitql.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/guxqdnezz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/ggyuxonfy.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/ggnjzatqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gcugrihyj.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gessirsgi.sHtML


<!-- 参考信息 -->