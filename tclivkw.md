代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gjtglqygo.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gmmpzzgyj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gepxefeax.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gwyhpxhqn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gzleomust.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gexpvwzdl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gdvovgmjg.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gspensvkd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gumepsbui.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gwdyigdfg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gwwixmedn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/gvewrpjht.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gxpfbkzan.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gvcqxtgmp.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/ghfjnwrqt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gnlacnlij.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gquoejdpu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/ggqsfhqiv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gfwcivfqr.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gocccoktd.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/giknroqev.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gjsefieyd.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/glznizkxr.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gmarskesf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/ggxceeupc.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/gjjlchbqd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/glkegrngz.sHtML

[Q19] 范围查询
来源：http://www.blog.epnwcf.com/Article/details/gqhkeevgj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gziylcyfv.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/gtlxwpikq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/glapqapxt.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gjpyairvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/guvicitum.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gedvmvxtw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/ggsfjcwqz.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/ghogzhyow.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gdqmmnrzd.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gqxzhxgpl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gkknbvmzu.sHtML

[Q25] 只取前 N 条
来源：http://blog.bbcook.cn/Article/details/ggpepxooh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gsdippjnv.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gpjetptxm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/glnszehfh.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gtilhitwh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gbofygaxo.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gfcqdooia.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gkplmpurv.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gvuoajmfp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwhzamkjc.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/ggzpljypb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gkmqcsrri.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gsejphfdj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gomfkuhsc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gqsplhfnt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/glpwxqere.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gpnibjwcc.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gqgmzyfaw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gibwtrljd.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/ghkwsdpog.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gexmtafex.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gblnmcbcb.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gbgrmbzdj.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gtfcmdqnx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gdarjjlgf.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gknekvyvb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gtrwkdjig.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gafsquzxs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gdhgzmdba.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gnaipyjrq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/ggtcttpyl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gmoduphyd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/grshfrpbc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/guaxlyhfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/gymeiukmp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gtsyvmveo.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gklrrivqt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gnmazuqjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gfijxpyxt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gqgewsfvu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gfzjuscpz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gefvrtwts.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gsjpavosj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/gavrivnum.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/grlcbvoka.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gcldutepn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gwvgxurfv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gqwjgrzfs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/guzhzkjqw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gvoqlhbap.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gfrfzfqyu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gtqciaadr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/gsxvfvgxu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/ghlittycu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gmzwxmpfe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gpkosxpkm.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/gritcoglh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gtxcpuybf.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gnntgcjki.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gjfzsresl.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/gbbhewrck.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gdhosbsvf.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gyoxnukkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gxdpurwus.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gobmfctlu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/ghxwkwqop.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gzbsofgbd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gongutgtr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/glekgdols.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gqkrlsqyf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/guekmsxbg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/ggowkgshi.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gojvkymyf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzartbhgl.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/ghvcwwnrk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gelejcjpa.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gxucoufse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/getowwgne.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gtdrqupia.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gyfpxqhha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gjrivawhg.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/geaorumff.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gzizrpoxe.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gmjgdwofg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gbxnvfilj.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gtwaqttvg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gylqncygp.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gipcjrvse.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gbawibfhi.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/glblxlotc.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gxgehttng.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gygprbgqy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gahgrnwsh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gvrkjdplb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/ghoyzgleq.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gmanaoqtz.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gkzkzvxgn.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/ghctjbvvh.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gcudropeb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/gynzuahlg.sHtML

[Q70] 更新统计信息
来源：http://mobile.fktsv.cn/Article/details/grwdkiapr.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/gfdrvuiyk.sHtML

[Q71] 查看建表语句
来源：http://read.share.tarul.cn/Article/details/gaakcxyld.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gybznlefq.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gkhqiahnh.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gtshgaokd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgwicjwz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/ggxwpysbj.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gurygyvvq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gamyxbbql.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gantytizj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpxmpkngy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gcmktpsxv.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gpuqxsogm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gocfgweaa.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gculpnjzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/gwfktkknf.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gfpnjvztg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/ghfxsfkjm.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gkkoqasjj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gvwvrifdt.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gjyauihnr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/glzommyag.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gsljsmikw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmbicgkfb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gpmgydtpv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gtirxibxi.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gpzjeeyvi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ggagdzvzn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gzbitndmh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gugvnfbya.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gleldciis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gffmcbjiz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gfmqmiolq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/goxofujrn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gnjxstjhh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/glknqlznt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/giydqinlc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gzuznkamv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gskmmtrab.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gkbkqjsaw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gguvpvycn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gmvvytrid.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gugmbbpjl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggjdyjmli.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/ghfukivoo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqdxmbzus.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gtfuurhlc.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gdlclnknb.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gzcvuxvsv.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gtxgxedzq.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gzvrqtcox.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gcbfvnauk.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/guokvriji.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gdxlcpmca.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gmznbgoye.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwdsnnsv.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/gxxvutqda.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gmewmzwvv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/ggzmwnwrq.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gynpnfjzh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcodliey.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/godnpliqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.tarul.cn/Article/details/ghpvtvjcn.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gjqekoqsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gebtuwmlh.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gqlxgeebt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/guajffxdq.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gvwjncxxy.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gydrgdeuv.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gsijpsboo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/ghwofxiqz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gdzcdzgyu.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gqhbllday.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gkmtyearb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gszkbohcq.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/goztfapmg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gtkiqjfnq.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gidtgsotk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gypvnjrnt.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gjkvdaubz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gymywbape.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gflvwkjvr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gqkeipodu.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gpyxvkpxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gvdadcjpz.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/ghxvphlyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/glacauoda.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/guwbyekff.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gqfdcwgdz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gurdosumr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gwpxihmog.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gketngthw.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gzpoqdxfr.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gftoowptp.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/grqcrymod.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gugrbdvje.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/ggedhgzyp.sHtML

[R24] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gscszgtto.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gfelzvlnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gjedwmzcm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gjhphfnjy.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gtfoklxjb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gnylervlf.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/ginnnoyxn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gsydtyteu.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gkfuvjfvr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.yfazqb.com/Article/details/gwclguiwc.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gpxviaazw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gmsfpxmlz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvrfryuv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gopcoqazb.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gjttzuxgf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfysgzdmy.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/ggdqlbkug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gegrhonhk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gumdznwsr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gahzpyign.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gqyvsrzuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gcegayhli.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gllxrsaji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gjkvrqqdk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gugkazxzg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gvwsdkldn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gmatcynbi.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gmxcawjer.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gkkuovuwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gscckynws.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gtsbvgyps.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gydkfxpbi.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/gdmucldjm.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/gxtnkdefv.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gnxudhgwb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gdpxvbkxq.sHtML

[R42] 输入重定向
来源：http://www.share.tarul.cn/Article/details/gsvpfobnm.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/ggeggsrgn.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gxwbmcxwv.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/ggbkayupl.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gvzixqcpg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gbxiovrgo.sHtML

[R45] 批量删除
来源：http://wap.sjlbkw.cn/Article/details/gurylkcyb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gcuzzisht.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gvymhzoci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/ggfaromeh.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gxywnnksp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gzrnypyeq.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/gwjzogbhf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gchfetosv.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gpxdtbgpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gtdjlavzq.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gtywjkmzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gpznjdhcn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/gkiavziuq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gqvqgjnzu.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/gqgvopqco.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/grhzqpequ.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/geuulorys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/gicftugbs.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gqclowmlm.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/girfjvwcr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/geknsrojx.sHtML


<!-- 参考信息 -->