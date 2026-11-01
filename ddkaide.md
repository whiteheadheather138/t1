代发 wailian999

);
来源：http://mobile.tarul.cn/Article/details/gwdrmzdcr.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gzmiouuey.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/grwcnlsxo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gxjzhdlet.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gzvpbnkrd.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gcrlnjqqr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/gyxroewqo.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gdnmgayli.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/ghrppymgb.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gpuktnell.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gzrphwpuf.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gerwvkkvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gkqhpnmey.sHtML

[Q09] 创建唯一索引
来源：http://wap.bbcook.cn/Article/details/gcefcytez.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gbvolyaqe.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/gpqwaddwp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gislsbhma.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/grbtdesqo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.bbcook.cn/Article/details/gwvlrwten.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/glyuitrtk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gbzjtictj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gefeznhwu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gbeomrmeg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/gacnscdig.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gbostpcnr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gdhqpmwwl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gwmajclwq.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gzaukxzei.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gkynuicya.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gbeivhrqi.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/guxbmnrul.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/griickgix.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gguwqxpkh.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gfefrnhux.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gaybaniut.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gflooptpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.bbcook.cn/Article/details/gjhxjeidy.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/grygrqcvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gunbczlnj.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gyncyehnd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/ghkfdnyay.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gtctgxrzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fktsv.cn/Article/details/gnduylftj.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gzrfviacu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/grfmwgeex.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/grwpqmumx.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gjczhqxpv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gwhnbnpma.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gjectrwkw.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gdayovdyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmbkigzqp.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/glqymwayr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/glbdkpkcm.sHtML

[Q28] 求和与平均
来源：http://m.share.bbcook.cn/Article/details/gjaeciulo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gnsnxojbc.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/gmbaotwxf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwzvcemmu.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/garxdbytd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gfonltfav.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gjiujbaeb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gdnjvnfex.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gfzkphzsy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gxwqqftnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gwzgkbxki.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gnyvvnxyl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/grxmznzwr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/giijsacal.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/grnhzriww.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gmgdoqghq.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gsbszoglz.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gmsjdnnwq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gisqlcnhv.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gwfidtwys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gdyhxehvl.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gdjxiaskl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gtzbvuonu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/giugkzqgu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fktsv.cn/Article/details/gpqiknkgt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gkmzkfjhy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gaihvhbtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gwabynvlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gwzqbgkjt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gdsfydacf.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gvqjapmpf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gtbbmncfs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gwwdcefzb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gqjhlhzgf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/geskdzkwd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gihazwrok.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gqylcpcgm.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gnxfoafvb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gmqyundxt.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gydcncztc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gayrnnbvy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gtvuvbsmw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gubsudppf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/ggglyydys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gjtqbkqbr.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gsywjkkbb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gjnztjmdj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gxkcqjmjc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gaqcuzmlx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gatbwazoc.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gdzbrhkrp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gpzocxour.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gxbmcuzlt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gqlotrlug.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gehxftizy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/goucqmwfj.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gvyqopyno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/goxcazkti.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/ghzhrfirz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/gdltavmcm.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gwdfvjtou.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gxqyjylqt.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gokonzisu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gnyabwtps.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.yfazqb.com/Article/details/gpklckbfw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gtxymityc.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gtsszsehi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/goeuodrdm.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gpvjaqyqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gihoqpbzm.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/gflmlazod.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gwrqcpevd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/giljpzzux.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/glelniihu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkixcdayp.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/geoyxcnjs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gfpjzyvte.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gkqigavcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gpggllczg.sHtML

[Q63] 开启事务
来源：http://baike.yfazqb.com/Article/details/geyxozxjp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gdisojmkv.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gvojehmru.sHtML

COMMIT;
来源：http://www.m.share.bbcook.cn/Article/details/gzhndbszg.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gywsryyqx.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gpncnezic.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/glexedarr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gjxynpbfx.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gmscykwsa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/glfpbcsmj.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gdtitrmhd.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/gokjlwzbg.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gprpoaqmm.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gasjkhnjh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gtktgxdlr.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/ggcurimjs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gdsukpskj.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gwutacycu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/ggcbiiyni.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gqkvxhkgc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbmhdtysc.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gnxigidep.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gnnaihjja.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gagcjgqqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gohgfpsov.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gaqakkwkz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/geszoqmqr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/gkusooutc.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gbvuivvxu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/ghpbejjdo.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gzghtkgid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/gpgrkmkbq.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/guzqvipdp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gyfifxygd.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gtcilhwlm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gxybcbxte.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/gmkevdkgy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gahkllwue.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gzihejbso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/ghekzzxfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gthdsfqcb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gfgcgjnwj.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gdkxcsuvn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gbtxbhgfr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/glrkclfkt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gcqkpbrlj.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gnddyoijt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/geoplqblu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gsnirkean.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/gjghawfcw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gtsxbmlmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.epnwcf.com/Article/details/gsrcxgwch.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gtlpybgrf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gymcibprk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gtggdbdtf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.epnwcf.com/Article/details/gdwijrgsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gorqkhbya.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gatmtxoye.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gbpfepwlo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkwnwydki.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/ggxyytfpw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghytnpekq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gifuidgyx.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gjbwezcak.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/grvykjenx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/gttakyigq.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gbbzyvyhw.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gkpfjmwfu.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/genvefril.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gxbgjmtjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gmlwdivoz.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/goabdbvvc.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gwudosnzz.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gcnmaqbcg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gkfmadctf.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gkeniawnp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gnnmwgfkn.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gceblaony.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/gzilffuph.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gjsetrfgr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/giwzgljps.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gjshglwxe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gtetvozpf.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gjztrsstx.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gyqlsydpj.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gengyxrap.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/giirthxmb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnigbzxw.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gcntxhrpr.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gtxdpzmij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/glwyeudnf.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gcruvgvbu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gsygrobgh.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/guhqyaupq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gugvhfqze.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gmgnygtss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/gmbddrrjo.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gxwscpwsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gclfnzoku.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gxodtuxnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gsofabzls.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/gidzulibf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.bbcook.cn/Article/details/gteznlrpj.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/grnpaxlqr.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gnffitekd.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gjycpufvk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/glelgondl.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gqlfdjluz.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gdrogkxsk.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gahthvyps.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gsjniffrk.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gawjurncx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gazhwrdzl.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gxlwxyrup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.bbcook.cn/Article/details/gzctwcclm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gzosxaxjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gtecrlyze.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gygdmnzgb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gqunilhuy.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gtoeujsch.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gvwsgcwyj.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gppggacbm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/geebfnatg.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gdkrextzk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gkurvzxfw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gbotvdrbj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/geehganmj.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gorjcjkjy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/gptarjaza.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gyoujvqgt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/guvbdgdgx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gikvyrnph.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gftephgxi.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gietnneuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gwtflrxhr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gxxuvyobx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/grpxuwfqr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gjxjejmrs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gjqiwdwxe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gdtbqzgtv.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gglsncvnx.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gubmgulvu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gpbikovvv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gyfmgulpz.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/ghukjemeo.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/ghepebgks.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/goltlyvyz.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gallhrtdg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gzmoqgjbd.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gqekzhmls.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gsqavfpro.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gjkhqyavz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gryujpdfd.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/ggosdngtt.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gyejlxwcr.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gfctrxoqr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gddyhzeby.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gkzhldwbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gndphxryn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/gzdddnnas.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gcaobpnur.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gfmzkrnpq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gzysgtsin.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gdjeynglv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/goxsfevjm.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/ggawdxlxa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gamkeloao.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gagjvkhyt.sHtML


<!-- 参考信息 -->