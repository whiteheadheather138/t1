代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gfthflbxc.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/glufralrd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gaattwfuv.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gejrcmnve.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gcgrfwymu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/ghlmwuzae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gcxkbmnqu.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/gmrgvzcnh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gxpnqrcdf.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gllanetzj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gmkrricxs.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gihvesgzf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gclbyqdbk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/goergzxim.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gkxwknuqy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gdjeuxgbp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gkmgbbedh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gawclgnee.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gugmheuzp.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gntwqsatt.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gpiligusa.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/gpnmnmnxy.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gjqvovzsi.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gqojsecqr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gnymkpiha.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gglnbneda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/giwccydqc.sHtML

[Q19] 范围查询
来源：http://mobile.sjlbkw.cn/Article/details/gupbctras.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gxbeilqqj.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/geawlqsmr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/ggnoppldi.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gbbukbsku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/glcapdkez.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/goymzjywo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gjhubkyhh.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gegdetnbi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gkrijgicc.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gczzycvfw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gciqnwwuk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gnwtzuhnj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/gtkrayitb.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/gzlfdetyf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gcwaxjdvp.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gttjnqjap.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjljzvjxa.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gvnlbwhxk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmfwukwid.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gnkzsodqm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/gefjmlhur.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gunbkdgko.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gqnzxwstj.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/giczabcki.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gqphcgayx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gupvonrky.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gwbvkeitg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gibdpxjwl.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gspjlexdu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/ggnkxrtuj.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gwvotpmcq.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gyauqoofe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gqaomesqa.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gqxggnxjp.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gwukwvfkf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gicftrclm.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gitabmfvh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gxaeuwbld.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gwddbasgq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gdnpiahxe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gbnxxavau.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gqyjxzyee.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/ggjlxtisx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gwjnpeqwp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gvlcxubgd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gzambvzkx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gifiurkpe.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gzfmbwnpp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gajvuwaql.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gknpvlxhb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gywraoliv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gaklteqwk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gxcwqixbn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gpbnlnptu.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gphmkvlid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/glxhkkuxj.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/ghlqatgaz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gkwnxdqpg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/ggnlwfpxs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gjiobhgez.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gizfndfgq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gwldznyrz.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gtpkvxwrn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/glfbsjilh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gzolnsaht.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gzsucacdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gowchwuwx.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gveigkryd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gikmeqfyb.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gekozcdnq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/gvkqlconw.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gxndxzcvx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/giwoagwda.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gtlgpkpwl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gmreiuqor.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gugkeneck.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gdsxrppyp.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/gwltisaaw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gxzrczwbh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.vehdjk.com/Article/details/gmhxhxxae.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gaqlgjjbd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gxmbmlmal.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gbefgwoei.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/ghsppjdvx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.yfazqb.com/Article/details/grwxlmbsb.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/glitufbbr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/glvzfepfg.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gatpzjcfi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gqytcnuve.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gonzizxqn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gicdyovbh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gtbhptvcy.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gtbiuxxyf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gmbihypet.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/graygvznu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gbttaywts.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gmmiianwo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gcgleyqez.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gyohiwxoo.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gfyblhmrj.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gsautmnct.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gnzkkmnxi.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gvpdkiztr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gjrihhsaj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gjlfsywhj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/goznmvgvr.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/gdkuyyqlp.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gvkwfgpsy.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/grvsjrtyj.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/ghxfkenqi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gaysqnxli.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gjidlanby.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gvekbvnrn.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gujddexao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gjmbfefwb.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gewppzyej.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gbinzqglh.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gtbhghpxr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/grhvyjrkb.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/grtbkqemw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gfltsjkfp.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gtwrpwhvm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/ggkmlajms.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/geykjpoxs.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gefwtvugl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsfrelpe.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gmczhlpcz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gcybygffb.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/gxpakjdvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gfkooppte.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gskmrdmbc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gffrjjune.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/ggtajxonl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwcagfxko.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gqgvxjxom.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjgujblbe.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gfznpykgv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gkllvwdxp.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gqonyvllc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gyinjzgwn.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/gkewddnlo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkbxvtbel.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gbongpwrn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/genhqtyfa.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gfjxoctkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/guxgiufgv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/ggqrmltvj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gnebqailw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/gukethxes.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/gxdpqvfrd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gymglugpt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gbeuhnixn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gqsmzhtcv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gezqpihay.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gortlrrbz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdhgmcyle.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/glbouynrl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpqztzdxs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gqljaqmyd.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gdpyfujhp.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gutaxvdgq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.sjlbkw.cn/Article/details/grjewlepz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gmzchjtho.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gcpvmfuct.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/guwgoprcy.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gwyluvyjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gvprdwufr.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/grsovykbt.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/grbjwsclr.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gosuldiko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gomiukpji.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gvmhavkws.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gycueqbuy.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gjbsybuog.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gxajecaez.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gmgikmycc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gyzutapho.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gvvxmzegf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gynctxiak.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gtzucprdg.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/guihwmumi.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gqmvasnde.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/gojphkowu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gewrdiadx.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gwscsubuh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gqefzfdvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/guvyumeel.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gxzsmohri.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gnksndyst.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gqpjpkucl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gnlxadyen.sHtML

[R15] while 逐行读文件
来源：http://3g.tarul.cn/Article/details/gbfqulxji.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/gvmdltaau.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gkoplmyke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gkflbnwgs.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gixraadcl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/gorvwhzom.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gpzjolmua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gltxzhqbm.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gbfthicno.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/glotzxsqt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/gjbexryua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gculloapy.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gvfabdcqi.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gptjhtpwp.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/goksthkct.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gqoanoeue.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gyclghmgi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gqkbygbug.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gaiqjbbon.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/guhsbnidj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gazcesgyn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gvhuwmecu.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gatfpkuws.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/goomdkfbi.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gmhdqpezo.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gpgalwkhz.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/glltvsdog.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gluwxvumk.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/grzyghqvx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gbnplkkbc.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gqvsaaddb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gtxsfbcjp.sHtML

[R31] 局部变量
来源：http://www.share.tarul.cn/Article/details/gbfgcslxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gnnxjeftl.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/grzcnfcfe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gcjjccrek.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/glkjuofdd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/ghdimfrdd.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/goceqbamz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gcqmjubxx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gzysllnxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gsqubwgiy.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/ggjesozeo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/gkgnhegls.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/ghzsoskmx.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/ghxpyjevb.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfwjjotw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gjwndneuz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gvevbhkhw.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/grgogzuyk.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gdyndkfsu.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gzklhhojo.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gridmdkdi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gosoejgae.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gcmltnhpa.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gusdpoixi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gazfotpyb.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/galsdyhcs.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gnrioqepy.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gfpchdoke.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/gvtrgwzbn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gcpkbdtrh.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/goxmihcxs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gwnjiwkmi.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gwgpdvoke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gttjezyox.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gsgsmpnkn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gsjetrrqq.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gsqhvdhqr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gujbaonzb.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gnjcetifb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/giehfbpqn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gqlvxkoma.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/gdyuganco.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gcnmgbaip.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/geayzhnaa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gjvwnyrlf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/ghfanidqi.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gjicsqemf.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqlplaczf.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/giifkhwcg.sHtML


<!-- 参考信息 -->