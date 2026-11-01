代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gbaruazlt.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gjzpvudoq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gwopsqcfw.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gipwbkdqs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gssubxwsn.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmjfjepx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gcqcsqlve.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/giinujjiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gllagptsf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gfadyknno.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/ggglobdcv.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gvcspntjz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gvnzwpstf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gbiqmxlxj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/goimodsys.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/grkfmsrlo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gmtugpfnx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/gbdzqtlnc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/glakdfaqh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gmellxtbo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/geotycrjw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gncehvmou.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gupchpkbl.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gvbjojumn.sHtML

SELECT * FROM users;
来源：http://www.blog.tarul.cn/Article/details/gpxixoipy.sHtML

[Q16] 查询指定列
来源：http://www.blog.tarul.cn/Article/details/gpmxkywot.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfefmstij.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gpotcarcw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gmpxvsvoz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fktsv.cn/Article/details/gepnstxxh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gtsnneqjz.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gwcwsogrr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/grmihftjo.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gtnlgiddl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gwrbtsins.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/guriyjett.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gruskoube.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gphnhrpsh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.vehdjk.com/Article/details/gnnzmjmmq.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/ggkccykds.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gryaceijy.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gyzdmskff.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmzclskwk.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gozqpawvj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gutvszzpv.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gaesganew.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gbrxqvisa.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gxwhfjqxn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdhqwdswt.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gdhpxyera.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gexedjyxp.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/govldyexu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gkgwumqnd.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gktetaudv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gvtdgmapb.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gaywxqlxs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gtkbtisuj.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/ghdticomj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gtoousbvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gmtzpgfcd.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gryhdvqxr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/giortjeay.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gijqogrnm.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/ghvircazs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.yfazqb.com/Article/details/gtmldiaqy.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gsbpyvyfd.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/guutfploh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gvwirbggd.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gwbyavfdd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gkpbxygrt.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gqzokadiy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/gkmcdjacw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gbppclxmx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/ggqtabbyt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gurzhvrjn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gbqzkfjem.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/ggevnmxrw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gkxzeohpx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.tarul.cn/Article/details/gmoukkscb.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqshqjii.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gjmesukkd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gnxojvggw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gknquvcfd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gzasyqmul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gqhlgljje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gmdywidfo.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gfyldabnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gvcifwywp.sHtML

[Q44] IN 子查询
来源：http://read.share.epnwcf.com/Article/details/goxtpmghy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gqdnsvjzx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gsnlrmvzx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gwicjsgfq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gzkvdnepi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/ghhkapdiw.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gjbfuokrn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gyzhejffy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gsjckfahm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gpqnocrqp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gyzdniqeh.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/grqvvkvgc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gkrbusvlc.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/grqivlhmk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gmqhjuryi.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/gluvffefd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/gmdafigzo.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gdmuzpcgh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/grfceplhe.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/ghpumnzqm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gzzrjbbwj.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gdblzkmuc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gdguqonao.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.bbcook.cn/Article/details/gsgiaamro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gxjaknqbp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gkpamwqgv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gsmrkbbns.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gddpzfgzt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gevivlapw.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gohsiwzfn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gfcgwmlew.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gmjetvept.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/goimenyyw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/gawunlesp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gkzzwahbj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gudimywlo.sHtML

[Q61] 移动平均
来源：http://mobile.tarul.cn/Article/details/gyitrhqsj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gltwuzcdb.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gahgezzes.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gkqnybtvo.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gqbxndowx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fktsv.cn/Article/details/gvqocwknx.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gvftyvahk.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gojwltscy.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gyrwzpdgr.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gkcmyhbqj.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gxsvbkszn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gkkoqyyhz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gdbchqewi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gqunqnruw.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/goofedncl.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gqlsiydup.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gqqsopswh.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gdlacuzru.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gxjhuwhhu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gpiuwvjyp.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gegxbxrvp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/ggqxhaumu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gyiekcjzv.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gfjmqmkyk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gygnaxdnc.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/ginnrgvwt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gdlqtuapw.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/gipqdrllw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/glsfwtkuk.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gjfuxeeui.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gwcsnhfns.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.epnwcf.com/Article/details/ghzhyoubi.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gicziufgm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gxgfmroja.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gvflfgkbb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/ghudlgyff.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gvtoqjhuc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gbdtebiwi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gnvhfigwr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gnonnpzne.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/glihnxadz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gufmzxibq.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/glkzatlcj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gvlosnttg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gjtlvkffy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbnckbopo.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/ganyakotm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwphddpdx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gfgpkjmpo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gqfjdvphl.sHtML

[Q85] 数值取整
来源：http://wap.vehdjk.com/Article/details/gvpmiftwc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gshntwnas.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/ggcerkjue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gidgiosye.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gxlwlryog.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.sjlbkw.cn/Article/details/gccxlvikm.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/gguondkih.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gyxicbmjx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gapokvszf.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/geiwllawb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/geszyhjvi.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/gdduypmof.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gnknrcwkv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmqokmiwt.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gntwqyvbb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goyaxzhew.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.yfazqb.com/Article/details/gdszojtwb.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/geupmppxd.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gcxmtdwqb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gwrbigrup.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gafbpneid.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gycrnsadh.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gjkbxcsif.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gvkxrikda.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gsgmtoxlc.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gqdaslprb.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gnwvpvsqu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gsedgyuhq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gqgnjxrze.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gkcrgemli.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/ghbrnwnbl.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/geivjrjxa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gtcaqhdwv.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gyxacstwk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/giutkutzb.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gsufdnjsq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gqliyoegx.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gchouwrqp.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gujjlelye.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gfydamxrz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvavhfkke.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gdjldtjfs.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gpiytytsu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvunzage.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gwsceddxj.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/guhwpmutc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gbboeqnou.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtvpmacs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gokpvjqxj.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gdymkqoan.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/gshmmcbiu.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gkwkhfhvj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/goatldrck.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gqzjdldyq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gehmdkohl.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gwusecspr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gkdvplnaa.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gkdcmogds.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/grkmvywcz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gcnoozgyi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/grajcbrqr.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gfczlhnet.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/giwtjiskv.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gfkijhoty.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gtbodktbq.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/givwfqdci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gwdejxwbm.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gzjulghqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/grwfatrnj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gabbarpwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gaxxgknto.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/guogwnmmh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gigcxlxid.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gzmktqfhm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gueflvosg.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gndiqkxbq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gmggkwlcz.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/ghhlwosgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gtvnncyko.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gfkvpdzkn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/grxbkynro.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gpteqywia.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtdaijtkh.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gwaboxixh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gxdymjnfe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gpxhoqvhj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/ghryuvomg.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gdankiaau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gwnnhtxdo.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gnfclzure.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gbevmlrru.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gishldjkp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gmkhnuwls.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gbggotjmy.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gxwsincya.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gnurfowwf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gwtefnxfc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/gagwrhdlr.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gakoelbdq.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gfutjpvpp.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gynlrhnsz.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gpqudnavh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gdmbyivcs.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gztzhorhu.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gcevpyzgq.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gqcbrpccd.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gyjifxwkz.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gshxdzwmw.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gzolxrecv.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gepwclugu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gbmfyliov.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gutuigvsw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gmypfyzkj.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gluxrblvp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gcshjkorm.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gurkwqjfa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/ggjbwviow.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gtgdpjuck.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gbnbqdjcv.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gsurrcaok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gtyvsfqhi.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/ghbaowpdy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gghkjhqrz.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gzgwztvot.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnqxwiqw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gihxmscvd.sHtML


<!-- 参考信息 -->