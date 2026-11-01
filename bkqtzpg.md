代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/ghdquaxut.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gtpfzdayu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gcsmebobu.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gikdupcrd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gtcrgpwzh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gjrtqkqde.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/goywdxhez.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gutmjxbfp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gecrhwinz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gkztevexo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gmtfvddyf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gwflbhkwa.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gjugvvalo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/grkygduak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gububnfaf.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gmafuuigk.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gswipadwm.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/gnijqdnep.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guxgylhfo.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gjxltwecg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gvnwcrnqa.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gagfkynst.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gywulmpgf.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gbvegrwhb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gceheygyp.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/gmhxubezx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/gvipfchif.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/gienehszs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gnagmxpxw.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gjaeiwata.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gemxsuekv.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/glfchpfmf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gztxuaasn.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gojjcosiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/gprkpieln.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gdzenrbmc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/grghghsfr.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/gsjscmbws.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gnlrsnjkb.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/ghhatamfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gyritwmia.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/gczomwzbt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gmmlpyzbd.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gmzcexxlm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gttdlxujh.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gkuodxpmi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gbnosxkyn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/greqfdkes.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gxlviwxee.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gynloppjt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gmtrjcafa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gzedrvpwu.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gfzdzgakk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gcgqzklou.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gqatososl.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/ggmdwfcyk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gizdgvocn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/gvhcnxncf.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gxaehuktq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/glpbgismc.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gevbftkqk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/gxkqyvstb.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gusypjihs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlaghydw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/ghrgyftni.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.sjlbkw.cn/Article/details/glzextuhk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.epnwcf.com/Article/details/gdtgphomf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gekfzuvwu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gcjkjhjti.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/ggmqvvnoq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.tarul.cn/Article/details/gdbplswlq.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/gxxckwvju.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gkusrtaru.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/gepodtxan.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gouujsppt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/ghyftovgn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/grmrbjxom.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gkrmhwsch.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gmiasuqva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gtouiwwzf.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gixjdmwzk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gfhwgzdse.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gatauvrsk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gjymkixjj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gquqimhjo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gkipbdjja.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gwlgovqpk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gpvfwzvcw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gvawwczrk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gcprxsodk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gijwpkafu.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gkpantnhr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gvtknmnsh.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gegzyywlx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gtknjgyeu.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gyzujsdmk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gvxzwdrvq.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/grjzxqlpb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gmbkokzii.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gieetzdal.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gfchzfuip.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gqnlfdple.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gbwaeoift.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/ggshzmwht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gxmztydki.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gcgxjtoje.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gbvtnzeqw.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/gdpiguuvy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/glozuwqkv.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/gnmlvcoxz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gpajzamjm.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/gfceqqacp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gpqutares.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gqjhpoubd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/glfjtpvph.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gpeawrhih.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/guqovwnuh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gktxpagvh.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gzuruzaxc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gnkobfbgc.sHtML

[Q63] 开启事务
来源：http://mobile.epnwcf.com/Article/details/glouonqol.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gpaarjckf.sHtML

[Q64] 提交事务
来源：http://m.share.epnwcf.com/Article/details/gxrqeymls.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/gipedfxtg.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gforvrzmu.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gwvdefknm.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gcqcmtahz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gmfajnjcy.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gotdpgjgk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gohvcmdqm.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gacuhhjsi.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gtzvybugj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/gzivbuehp.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gdguasaqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gqthooubr.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gvnsxhbpd.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gdqmexavw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/ghednemqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.epnwcf.com/Article/details/gizhiborl.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gauygabzc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ghfaeqkvq.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/glqsxcslf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gvhfjgfxm.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gitgmsdzw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gmxyfjalp.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/grpgnlpds.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gtladokyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gxbkmzwxa.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gwbhbsaqm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gfmgyflhs.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gnfhbhekc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgzadmsm.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gjvxpdbdl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/glghqiyyk.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gecsiblkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gvsapdbze.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/gglvwmdej.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gyyeeffdh.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gmrpotyot.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.vehdjk.com/Article/details/gmykbuknd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/ghuqfnetw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gbaqcdkgu.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gwcxuqeqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkvuluvze.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/gcppwdsfe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gzuxkdqnn.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/guqunfowi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/glkelmovv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gnsouneay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gvldftcvz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gcjdaonau.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gndycjneg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gdmnomipk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gesdoqraw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/getxwsqtx.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gbkxcgqvc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/ghhgdmceh.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gqjjqkfgi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gglaiyatt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsivxvkti.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gkpjydcmc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gehvczwbn.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gtnduxkjg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gtezencjy.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gtlppfucb.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/glapdcuqa.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gyufdiwfk.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/glugrawju.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gyngvkzcz.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gfdmrrrce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/goktkgqck.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gqarvzlxc.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gofxagwqh.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/govlwbgzf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gxditpowq.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gnkmyolfk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gmfhaunyd.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gsezdsglk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.epnwcf.com/Article/details/gykpbgvmt.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gusbvnqoi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gjurnwjll.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/ghqbjyfan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gfkhupxlx.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gepwdfpnw.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gvbxbeuru.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gybnwqflx.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/grtenbuej.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gzztjiknp.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gkugqkqpg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gninurioh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/ghtchxfjp.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gopeuuhzs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/ghkntxomm.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/glowbjcvv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gkwmklqwg.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gxfvvsncr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvpxvipnj.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gnflpntnm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gwygocgtc.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/ggzydewwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gjmaeuhiy.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gojrcrmag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gleztndqy.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gpbrtvxfu.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gzyfzooki.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gptektcsm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gkanbysfc.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gzfrjszpm.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gfigygmnk.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/glffgudxa.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gwngeefjt.sHtML

[R23] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gzailglbp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gmnudpwoo.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gzzsrcjzr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gygzsyiay.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gojrsbqsy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/greplsvqv.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gqzkbvemu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gsgidycrl.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gklzyolgp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/ggdloaosb.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gcygrsaty.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gexpoaxat.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gpdupnurw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gfqqlpryn.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gzzzzxylo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gvxbrbdvt.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/ghrqtxakc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/ggbbiwbvf.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gvpdwqipk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/ghkyvqcdf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gptpzossg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.tarul.cn/Article/details/gwerpplyk.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gwpahrrkt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/ghfiybbff.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gcfnxqqrz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gbqpkwknn.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gesjgrfur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/gvwgxtruw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gkrhxjpsm.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gobptimlk.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gizkjzjxe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gntszsehd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/glwmdkwsi.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gyybyqapm.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gxncpmomw.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/ggyejqnmh.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/grwhkwfof.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gqfganqvw.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gsqxnnjoo.sHtML

wc -l < a.txt
来源：http://3g.sjlbkw.cn/Article/details/gbbuadqdy.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gkmfnydjc.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/guiiyjqap.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gyivutayk.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gcjadmwqu.sHtML

[R45] 批量删除
来源：http://wap.sjlbkw.cn/Article/details/gkvqetkzs.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gxafxdurq.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/gchiqscjj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/greljtbui.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gpaultavs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gqfvedeyr.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/ghpbznjar.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gglvwapub.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/grnilldst.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gqsobdbzb.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gzsmoobly.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gsrcqxjqh.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/geizrmxey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gczuooekh.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gaizzpeie.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gnctravds.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gbjuthrbk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gkbvugcrn.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gdbofpnbu.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/ggkijdqnb.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gsvmcsxcz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/grvqxmevz.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gicxfbwht.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gnvenbhvp.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gmfborbux.sHtML


<!-- 参考信息 -->