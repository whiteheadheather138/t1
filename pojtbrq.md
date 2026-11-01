代发 wailian999

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/ghdldwgcl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gbzwfyvbi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gaxsvdfcs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gpmpikffu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gssdqhuhx.sHtML

);
来源：http://baike.fktsv.cn/Article/details/ggukufpao.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gnuytwrmc.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gzbqhpiqu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gezzdhqut.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gjclbwhii.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/glttqqhuv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/ghbmjbhgq.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/geroukaqw.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/ghimhysly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gzklughty.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/gnvtbiucl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gutgstehz.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gqfgqpjxo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/glgubckdh.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gfufocmav.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gsxaimjom.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/glfrwuyed.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/gspoznjrz.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/guyroufys.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/guwcjqrpw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gvurvcsdy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gbeswbrkd.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnrtjdaq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/giqgoxpgl.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gkordapgl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gnzfscngh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/geynbrkdf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gbullqflt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/ggjathklu.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gcitxoahl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gvgteisym.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gqawryeor.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gbsaweutg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gvgeaqkot.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gyhttiyvc.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/ggkgzljra.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gkcandpxu.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/gxfkzpkhq.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gplvbqtqf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/glhfbnfef.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/ggausnjmr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/ghacssnyv.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/grhjgntkt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gjgabvvts.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/geixwptzp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gpkfslews.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gzobghnqs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gfdedcydw.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/gbgxqjijy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gflozkfis.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gwnuomvui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gqoiipjew.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gnexnziku.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gpvryhjgs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gjoihlssr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gvaxzuffj.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gxtdepnzo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.tarul.cn/Article/details/gpnxzrqdc.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gdufaargp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gmjeqbthr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gudjpwgal.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gyinhbjzp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gfimkfroy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gpwkhtxco.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/grxtfaylr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/galqdfgqu.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/ghomjxqtf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gcexhcsbd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gvmqlbhdd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gxwumuuxq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/ggoyzkmrc.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gepirkqev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gguzfkfzg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gqnyxgbdv.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/gplprmjam.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gnozeqmcj.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gwzwonchd.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/gwuvvdwqp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gxfhjjeku.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gqkyeeqze.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gxodozhox.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/gffsrilkj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gliubqmkn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gotyvbwlj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gobozwadm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gpcsygalm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gwwdhsqyh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gkjvsyapg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/ggyjuxdyr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gjpiuqeoo.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gjiznqbfc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gktrmhzjm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/grjckxkpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gtfcbvpnx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/ggruwnusb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gmhffbrhk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/gnytlkipq.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/gnfioiqor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/ggvzojqfc.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/gkybqnofo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gfjfrtvbr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gwtupfghg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gzkibqqsm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/gvwpaprmy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gpqeypsir.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gurcmcchq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gsgbvakcr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gmwsnvvpj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gabmhstpg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fktsv.cn/Article/details/gybkllbiu.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gyzgpgueh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/grzeklfic.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gkrkcewea.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gwnojlvgf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gcjrvsvki.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gqbwulcys.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gbbunpfqb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gxkirfqpp.sHtML

[Q53] 按条件删除
来源：http://baike.bbcook.cn/Article/details/goygnhgln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gpdmemxyu.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/grklvncui.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/glwldtuwi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gbbfbbmee.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gdfpiaysn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gwcbgwqdf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gkvbbuyqi.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gktwvobyu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gigcjnmfc.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gvlgtczak.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ggfdtmryi.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/guqezaudh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gttubamqi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/grkeccewa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/grdndbdft.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsyfclzsk.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/goxsbgcen.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gakpsqflt.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gzgadusjb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gvdjkayvq.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gpwjvgudt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gskjhimab.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gtjdmfdxw.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gtofwqbqp.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/goendnkfy.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gohtcrwou.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gbqgewlqy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gtuhpgrqf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gvkulyfxk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/goiehubfa.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gjmknlfsn.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gqxnsieos.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gmgasqglp.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gqgwqfkru.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwdwgybe.sHtML

[Q70] 更新统计信息
来源：http://mobile.vehdjk.com/Article/details/gkkbydcvz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gwhwodceb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/ghqpdphzh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/grvbduijm.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gaadwzwnx.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/glztnbkkm.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gukihnuim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/grqfwmyvu.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gugqkowum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gupyvxqte.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gzcmywdii.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gneygshwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gkxgxoavr.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/grzknrldi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gohgbkwxh.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gjtzqwpqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/ghpyrdhah.sHtML

[Q78] 当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gfegosjsi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/ggwsxjipa.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gxeuifzqv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/ghrnhonrj.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gmoveveqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/glokftkjo.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gwvcwjvtw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/ghlunwrjv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gigxhvvhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgibzwml.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gupmwkhmj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/galysjobj.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gxclkupxi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/giyuypyvd.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gbpjknkkl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gqlswbykq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gzjcercfp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gxuqrjphl.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gnmbzchnz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/glpujchjs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fktsv.cn/Article/details/gmvyhboau.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gbfxqnkyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/glzolkglr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gjdkegesi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gzowjghcq.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gdujpsxah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gackmyhhv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcvmurgwl.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/ghmukqvhe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gevqhclzh.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gtmwbncoy.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gqurqhefi.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gyhuzgsxf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/goaozcurm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gvmqwagum.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gxcalphsq.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/gmfswpuqx.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gsomrjadi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gihmyniqu.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/gwoagcwwn.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gffkhicxt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gzfoprfna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gomkiquzs.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gnvympmsj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gaixhsypw.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/godrrdzgc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fktsv.cn/Article/details/gckizcyub.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gbuberlwa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gkwbnydey.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/goqabajgy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.sjlbkw.cn/Article/details/grhkvvdpc.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/grenxqmpf.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gkcxmqhoa.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gzhgqphsp.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/guairimkz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gjscwvnty.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gwhnvfdfd.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/gvvbwnvwx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gimbcnjbn.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gbcsatppa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gtugqugei.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gdoduwhyi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gfyuxpdhf.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/goqwulaux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gcixclazf.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gjydlflcz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gviqdsfob.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gptsmviar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gggzmafcn.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gxiudgknp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gbivoswfq.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gblxkecdz.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gxwjjofrm.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gyhbcglth.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gtgdnrtwo.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/grpozstve.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/graimhtpf.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gqfysragr.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gwjndiovx.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/geknqfaoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gvzsbmjan.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfmhjlnbc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gpegsbglh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gjkcmlgaq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gnmawtadg.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/gmhjmjxbq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gnucogmys.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gddjtpfxo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.yfazqb.com/Article/details/gnoazetur.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gdfcvuczi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/ggoprnlwl.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gmwccfukg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gaslzdxjz.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gxpjxhodr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gbhgiwmmn.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gczbptudv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gryzykpup.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gvubgirma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gikhjdyoj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gmmhyfjdq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/glnkyrmat.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gdnyfbbnt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/ghbmfkpuf.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gtmoxprfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gwvdkpmql.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gwjjdkrjp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gcleqkklm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gnplqjilq.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gjrgdvwqt.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/grijvessb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gjequcqjn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gkqvzwgng.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gffsuwfny.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gequfczjo.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gwupwqtsa.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gaztvevye.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gtndfpfqq.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/garggrbok.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gjdexncpb.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/giurhyggg.sHtML

find . -name "*.log" -type f
来源：http://wap.fktsv.cn/Article/details/gbvbgkvwp.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gopmpeiej.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gqlewzpqq.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gyxffpevb.sHtML


<!-- 参考信息 -->