代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/geggmqquf.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gyttnqpuv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gveygfrjc.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gvhcqefxd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gyjlkzgyf.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gcipwxkrz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.epnwcf.com/Article/details/gsjjxuqza.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gltslpqaw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gvfqrivxy.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gfggrfirb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gbylbwsph.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gorfjkfib.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gengcogig.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gvoilzbuz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gzdonprat.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/glkzntabc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gfejujsns.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gimkhbkms.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/ggyhtvdyr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gwannmrvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gekwkfjmg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gfvqpvxnj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.yfazqb.com/Article/details/gweczcizu.sHtML

[Q15] 查询全部
来源：http://www.blog.sjlbkw.cn/Article/details/gkuwbuwkt.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwdxrbodi.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gxwucnazn.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gfjecevap.sHtML

[Q17] 条件查询
来源：http://wap.bbcook.cn/Article/details/gpicsiyzs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/grvndppyj.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gtplxxuvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gomkflvog.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gsumpqndk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gxjxdfiej.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gilvhzwvu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gjeugkzxj.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/ghaabrktb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/gjezdcqbb.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gplloybtb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/glajcnpli.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gttbzibkj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gbhvaxzhf.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gdypqoffb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gotggdmeb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/grmnkyorn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gdaycttgb.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/grznrqeyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gudlsbsym.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/gkgccsjra.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gvzpyokaw.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/guwgemtia.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/ghlbgdeqj.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gdjiswssb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/gyusaidpl.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gqpbjnfju.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gluktwubp.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/glmaqueeg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gwtjzmmuy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gznzeaaen.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gomaozhja.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/gykqdooyl.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gngryvbfk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gqliehbdf.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gtdkzcdev.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gthogyalc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gnbrgpmtk.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gczaasvzq.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gbnzwwyfl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gxwaahigc.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gwyfgnlmz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gjhofjhhm.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/ghthxvvme.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gifftrupj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/giqvqtkwa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gxbbjotqy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/ggtmysewc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gdgeeknbm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gdaegmpxd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gqnxoawhb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gnzybxmyj.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gpzpxwssd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gsjuawzye.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/goacahjey.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gvhlivmln.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gmmflnkch.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gjfowviuo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gjzgthtif.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gfatyxzeb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.sjlbkw.cn/Article/details/ggmrhnsyb.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gorsfwghk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.yfazqb.com/Article/details/gfgdpbqxg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gxskrpdlx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gbnhgvwww.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gdwylkbsf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gtsuoygcv.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/ggiapjxrz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/gurkqlusb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gvvgfftjw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/gsofqlquv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/grskmrwfa.sHtML

[Q49] 更新单行
来源：http://read.share.yfazqb.com/Article/details/gvlhdaonq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gwdgvkaqt.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/glcjsaagp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gnmoclzio.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gglazgfwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gbotpiwxm.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gfdqxguix.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gmsnxsrvr.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gjjqhjxss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gbndmlyyk.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gzndcccsv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/ghcluukma.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/gawucdlgn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gyfokgjyy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gokiazcda.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gvalpgejz.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gllbvvuad.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gxbgnjqho.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/ghvnmudbz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gsskjwwqr.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gxmmqpydv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/ggzwouwue.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gwzgdvnos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gnrgvtuul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gbfwpzikl.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gajcklcof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/ghrrldrni.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gtgwiyoct.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gzihfbgye.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gsbwgwyam.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gbtdvhaao.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gbxqhpvmc.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gkgjaqtay.sHtML

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/gccjedjnf.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gjlrxmrst.sHtML

[Q66] 行锁查询
来源：http://read.share.yfazqb.com/Article/details/gqpatwrlx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gxzgkwnov.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gibsahbyr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gaxkbbomu.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gomfpeyif.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gqjlvbukz.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gwjmxxsod.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/guzgehgpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/giexdemvv.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gjwersorq.sHtML

ANALYZE TABLE users;
来源：http://m.share.vehdjk.com/Article/details/giaksozqf.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gemkmvgmg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/grtkikhqd.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gboxtkoik.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gleukofsj.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gzlhvfuaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gxtptvypp.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/grvwyhhxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gflduajej.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/ggriqqguf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjposmwc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/goggtcefv.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gqnaqoiwe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gnthnrfrj.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/grdelxdsz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gxvycfyil.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gqobawdgp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnardydq.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gwtuwyshs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/grzmazniy.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/gvvzzkquf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gcqmmnqns.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gzvaqsoue.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gdsgxuahj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gyjwihuue.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grpjltlfe.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gfbtundmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/goodwjzmt.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gzzvprkra.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gphtezgca.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/grchqszzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gnftqxcft.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gbxdrmtee.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gffldawlc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gcotlobnr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/grtkwpfbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/gasllximo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gyaatqgha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/glpxjcfja.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gjdqtlygh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gqmvnrtda.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gphsghycn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gyncceubw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkigcuweg.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gzmanjuqn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggdhieqcl.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gxtimqlao.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/grscnefvc.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gqeuhxudf.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gznmyltiq.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/ginlhcxfz.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/glkgkhpky.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gucxxggzx.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gfianvalf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gbwabkbhm.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/gmuxzcxvg.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gskujjyrv.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/geofsysyi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gtoukeizx.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gswfxxubo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gnuovtpug.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gucsuzwlm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/gqlgsmcte.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gudtrqptg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gaqegxxza.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/glsiqnunl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/glalheyto.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gmhhbbsty.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gsmtyisku.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gimjetalj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/glzwqlgwe.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/ggnhbuyzi.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gioxdyjyx.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gmelfkdfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gglpcdsil.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gkllkpkeo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gksjhxuoh.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gszvxgsij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gptrdmfnn.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gpmqwriro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gqerumcfp.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gmulqxrqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/grrnzchxn.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/grgspxwyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gwpfbeqpx.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gboyodurp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gjdzqcstb.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/glrtiuilc.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gebkvsioc.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gxdpwhnai.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gpbplunww.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gumfwjxki.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gcsndolfd.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gqecuuhxk.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gaxkemawl.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gcyczacsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gvbsuqcmm.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gswomgzsc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gkwaweuvq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gbptombba.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gzphvdbno.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gzgvahveg.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gdvrmiaat.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gwhwsklen.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gnwczesjd.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gqrqgebjc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gatzhhnrw.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/ghugqptnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gbnhegvnt.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gdmycdwzu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gfsorjvws.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gqcgyiqka.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gzzjhkaqe.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gagcxcjkk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gtvxpjhgs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gxacgxwoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gvowszlsp.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/givgbgdja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gmqwcnqpc.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gqsydzczz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/ggjsodrcm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/gxaojvgjo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gkgkabdxk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gsbpoerpf.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gptckapor.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gvnjspsbu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gquqhbaqc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gzldqcwjk.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gaoziluud.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gyieetnuo.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gqvxgpwli.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gpejtsfix.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gbjfhfucq.sHtML

[R42] 输入重定向
来源：http://baike.bbcook.cn/Article/details/gbxjwpoum.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/gsdvlnfab.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gdbunkwlf.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gflzmbyha.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gyhqserok.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/ghrkqopok.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gfzqdlsbu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gywfgvjct.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gzltckoga.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gebdvqxlh.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gxihkqbgh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gvzahplmd.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gwdemdesa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gkspnawei.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gsrrkpcmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gihhiqfqw.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gmnmziucj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gsahbuwta.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gtzfbdbxs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/goxvqbchu.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gkhfllgda.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gzqvxfkhl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gklaeavke.sHtML


<!-- 参考信息 -->