代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gvmafwasg.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gcgphvavg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gqgryhrjx.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gkzotzoyx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/grumfkjus.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/gqjcdzrwx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gjfthftpy.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gnusgbzqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gunjhtuuz.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gzawyyiju.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gjgrrmhso.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.tarul.cn/Article/details/ghpnrnqst.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fktsv.cn/Article/details/gocawczxv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gcoarnznp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gwsmcngod.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gmkgmosce.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gtmcxqnzl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gulxandah.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gdwgzlezs.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gljxkjywb.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gclzyuqgv.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gdpjoskme.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxvhqkzr.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gimfhmbss.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gozmhxmax.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gnrorahnm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gxkrjhpte.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gbaycbypi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gnqelujai.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gotargwsx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/ggzpakbxe.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/gmichtput.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gpngvqqpw.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/gqhntwjcc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gmncsymvo.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/gxyivqlbm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/girmjfzgu.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gplwjtjyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gqjapuphk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gkafubrhx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gyemgzbck.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gwdwmpuka.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gsytnizpq.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gyemppvaf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtgofrmfx.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/gncwbtnjg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gjlzuxivy.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/gefkedcdt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gughhobpk.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/ghiufweie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gkxldpxwo.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/glikqkrmb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbvcxpbv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/ghsotlgln.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gnygwgtoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gwjilkuij.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gxtujgibx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/ghduseyxl.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gwdkyqjfm.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gbdifjddx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/grjwyvnlw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gzvgspmsu.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gxafvubrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gnzkwhzdu.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gitvnyuko.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gishkxaem.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gbinvqasm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gzlxeaiic.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gfhhwgcyf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/gzvlppvtb.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/guhaojatu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/ghvwfhzex.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gcfgiwpzc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gbcvwsbzy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gipfhrndc.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gxgwuvice.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gkiinifvv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/ggzizcuvs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gldkdmrwc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gsjzfoanq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gnddyikvs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gciijmcpk.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gvxgclfau.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gkfplavqo.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gmwbjbqor.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/ghaghsvce.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/gavkxrrgl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gsmsgtscs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gaedfhjbj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gsmbqbhtn.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gsnltycjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.yfazqb.com/Article/details/gmpjioxsc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fktsv.cn/Article/details/gbdzviuvw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gefdruevy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/giwyhgeus.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gndgskqyt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gwmzvgmuu.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gkrurkrnm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gvgnayvsj.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/gmjukqlym.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsefspbk.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/glgigtpuy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gmuxyvqbp.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/gzmbuleoq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/glpqyghwx.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gqatbhxcw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gcqsfsxbg.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/guctbavai.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gsybvpskc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gnabrzahb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gzlymuewu.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gwxcuezsw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.epnwcf.com/Article/details/gqjjczwzn.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gvootgzhi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gkvukzxyg.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/goldahqas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gsckpmnui.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gbajpqjrs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/givuogxlx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gnwplpigd.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gvezdpdvd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gltercmgf.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/govrqvfet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gzhxpfbdh.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gwqnfwgbo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gskvjalbk.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/grqhgeckq.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gvnkchlwo.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gguadhtau.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gigozlswr.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gcwqacleg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gymsfrcef.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/gmfocnbij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gmibwyrvn.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gmvpauari.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gkulowpgk.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gvxpqowtc.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/gzlwnyoea.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gtlpnfhoj.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gipyqjlcy.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gszzxwmop.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/ghehkappw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gdtmwizuh.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gpeenlmgz.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gficmhbbn.sHtML

[Q73] 查看表状态
来源：http://wap.epnwcf.com/Article/details/gfzvhlech.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gdelxgnui.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gjtgcodup.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gmvqdlxhc.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gacwwoqij.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gsjffhgst.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gktngfzde.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/gpykeyvsw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.sjlbkw.cn/Article/details/gkvsrgylk.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/ggfezszub.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fktsv.cn/Article/details/gzxocjfzf.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gwabfpgma.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/guibtlldv.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gbxfvhqfv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gkjmbpgji.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gaddagovc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxibyldml.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gcncthdra.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/glmbqwipl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gpxmyzxht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzgbrymna.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gvmqvpkhi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gabagdpxa.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/guomzkfff.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gxtzrslsu.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gdrrujbun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.yfazqb.com/Article/details/gkagbqdqn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.yfazqb.com/Article/details/gvmixhxjk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/giaffiebr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gscppaqqm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gpqxtrerk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/ginulhrls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gsecmmwjy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gzkdffvtn.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gkhbvyjik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gffnicoxz.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/guoezthpd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gzuufxphw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpilofpfh.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gwxfzlbhq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glaawbtxn.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gsxmdqvuz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gecadjrus.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gacznyuzx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/giwneadzl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/glzxdfvhm.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/gyxbzlgvk.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/gvweswbau.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gxishpttj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gwfyiuowp.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/guqwynfpf.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gkijwfvul.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gnbmsylpj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gqsdhhvvb.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/grdooljde.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gkderknjc.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gigccunpw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/gpwtoyusk.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gegomwpiz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gpdolvvth.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gwkmgqtfs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gyoqcjbof.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gvunbkulp.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gwbjpfbnn.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gufgmyung.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/gfllhvrfc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gwiculzbj.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gpqsfloph.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gwjkvadug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gqrsduxqh.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gupxbmhzl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gjjanaksd.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gmswapjys.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gqvsgwhst.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gcxntiupu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmvgvqaji.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gjcjivrnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gbhojlmfh.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gygbnmetl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fktsv.cn/Article/details/grqemequs.sHtML

[R18] 遍历数组
来源：http://3g.vehdjk.com/Article/details/ghmxneshd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gfyinmmuy.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gkzvhtzpu.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gtegyuiav.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gsywsatfg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gibvehunz.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gswikhveh.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gyjxnfhdc.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gcmocwega.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gpepknzgy.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gqucuheuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gggrxirno.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gjtpqvhhv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/golrijpnl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gvvjzdiux.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/guxmdlniq.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gwpdndzuo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gnrowklof.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gicstafil.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/gpqgmnmnd.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/ggwrxyfbu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gxhrvkpjv.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gaizbvjow.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/ghhimxjgh.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gtxfyhrjk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gkxpfldan.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/garxholdk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzavtovx.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gldcegclm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gvnjoqdzg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gmvifaajw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/ghuvbztuc.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gpjhnssdn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gukgokagj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/goaamjizi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gqcbbiwuz.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gxafugyev.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/glvpgrnjv.sHtML

[R37] 把输出赋给变量
来源：http://3g.tarul.cn/Article/details/gzhvnvhui.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gwronrcwd.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gbfsgbdkz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/givchsnit.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gdrflfweo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gewnrxvfp.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gocpqujcv.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gnaqmkdbd.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gnmsaoplo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gvycltfqo.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/ghmvcdvgs.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gppnfwxej.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gfxyuibxa.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gcfsvseeq.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gzscxzdwn.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gcseetqno.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gmduqshuc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/geiretrbs.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gjlrkzetx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gapqbqetu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/guwavhppz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gucojjipj.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gupvyrifz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqkjablmo.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gfsecnwzi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gqonnpnje.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gposjyard.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gjllsjbfc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gqdhdltfs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/glbqywsjw.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/giqnardnm.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gxsufrtkq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gpaixgxmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/goiaiyctv.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gkbpnnlwy.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/ghvgbeuyz.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/geijzlmrn.sHtML


<!-- 参考信息 -->