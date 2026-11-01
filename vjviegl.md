代发 wailian999

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gyzpmqthl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gqlodnpix.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gblvejacb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gshthhehq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/ggmnsqycs.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gcyezpjtd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gdbprjiku.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gbxcmmabp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/ghvcdnerk.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/geusihenu.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gvgthffqw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gmiupkssp.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gtcjfznoc.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gyssgxbin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gzwbpkrwv.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/grguhkkfr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gtvdwcvms.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gmzdbusqd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gmgkhtvfw.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gjtbtkkca.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gehnoabde.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrhkpyen.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.vehdjk.com/Article/details/gakljhjyw.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/gyqxjmwjo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gwkbmygeh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gtidrgser.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/ggxflaeac.sHtML

[Q10] 插入单行
来源：http://www.m.share.tarul.cn/Article/details/gdawsffun.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/guylbhhwl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gocmsarjq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/ganrkeggb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gosamptqp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gvxlgdxvg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gzdvgxxht.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gewotjysq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gldbuwnbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/grxfxgaru.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/geuxnnnqm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gxjkahpse.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/grirvqelq.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gyzbggivc.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gxfbqlcpb.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gugksqwxx.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/gbldefunj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/gfanvussi.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gymauyeuy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/gtdyukbfh.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gzfebvnkt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gzkbughil.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gdknslblr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gqxaoetac.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/ggtpkrloc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/grcpwnbjn.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/gpzrjmofe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gtwpmvqbj.sHtML

[Q23] 分页
来源：http://wap.sjlbkw.cn/Article/details/gzclxlnyn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gkqrhhqfn.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gvlewbxbq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gszrneqif.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gpepyuozp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gjnonifcj.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gzcfuaqdw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gopuoidoe.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gidlgqwnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gfuilfnwd.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/guebetqap.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gfslpahqo.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gnnitybiv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gistqsfdk.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/gsbprrbyv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gcdsqirzq.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gtwvtclkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gmxdmipds.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gnxwsbnix.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gnpvntihg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gqrwyeysl.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gqolyhmsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.tarul.cn/Article/details/givefqgul.sHtML

[Q34] 每组取第一条
来源：http://blog.sjlbkw.cn/Article/details/goyopqnxj.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gucxsfrqw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gnqayhuki.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/giedkkqbq.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gjphmcwyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gupbeyhpb.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/gdjnjnvkg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gxmhomgez.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqolcswe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gssybyxrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gxpxfqmgy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gbgsvieqq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/gdfqxgfzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gybornvwh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/guolsuucw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gemqretgk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gjpemknut.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gredvegyy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gyczfxted.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gavkpduic.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/ggjewuhnq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gdvrqkmpb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gujxhextp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gnjcafblb.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gwljkuvxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gcliijvmk.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gbrzunxhh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/ghyxcdmfn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gwysrphcq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/ggsivnejr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gmzvkgdyq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gzmlpmuoz.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/giludenmj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gvdvczcru.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gorphvptw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gaguwpqnk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gbhcsnugg.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gkihlvbsm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gtvkiefpv.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gzxghtvob.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/ghkfohkxd.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/gptksyvpu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gvvsodccr.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gejrbjoat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/geixjepsp.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gtyuowrco.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gnegwvuzr.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gruclaugm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gzsqqbfps.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gorsxizqn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/ghxhkttdh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gextmymps.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/geosoadqv.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gmhrzstnh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/giateaqre.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gxxabzwuh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/grzhliqeq.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gabxnwhjf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gsresamsk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gneubxgzr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gwvxnifrh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/gchvwxifp.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gtpjzwedr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/grbxwhicm.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gcvyuiabm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/ggtmtzjnn.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/ghrentqqs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gullaeugf.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gcmqecseh.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gsnrkkpsx.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gzvajlcbh.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gmxkvbzvd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/grqsrsakz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gktwamkbu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/gwzzljqkd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/girdszfsn.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/girszvark.sHtML

SAVEPOINT sp1;
来源：http://3g.fktsv.cn/Article/details/gndirowcu.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gtvmhnmei.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/ghqugtyfg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gunceugkl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gyyhyzsls.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gwrwegjww.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/ggntyuylk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gyrurmulh.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gitiasypu.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gjhhjnsoh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwlpxzei.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gihtswreh.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gisrllqlj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/ghxubcyvr.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gjpofmutj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gyzwgnnwh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/gxazcagaa.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gxgbfpqtf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/geeuuzgxb.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gauxkwgse.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gwhnstpiw.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/gunvciqfa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gzcfvznrq.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gqmtolxav.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gjxbrawqs.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gndldfomo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gezkfpzbf.sHtML

[Q81] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gnvnymnlj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gyakzetcn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gcpjfdbce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gaqoxxamk.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gkntpdrkm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gdzklydki.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gocmzmiug.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gusykaken.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gquxbsbtv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/ghuqbpwvz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gvrqpjjlj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gzgmwvqcf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gobfzwbpp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gzheygdew.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gznyvjxhh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gfyckqlvx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/grjrmzdrr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gvduidqdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gdhcqczaq.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gqvbcakqf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gbfwtewdm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnrsjhlwg.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gjhkutkjl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjkuvsbyf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gidpeeffl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/ghamefmzj.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gwelvjivw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/ggmnrwkfl.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gqdfztbpg.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gtjcbvyro.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gplpdhhsn.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/glpzblhxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gmppcwyrx.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/goplojjec.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gunmpvknr.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/ggtrkblii.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gldbedldx.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/gbxdnaqah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gezrxkvsz.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gxppdntle.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gjbraysbu.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gkblcgnqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gdprcffjo.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gcckoihxa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gusmunqos.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gnicfvlwl.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gnegjbrbb.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gygdgkkzg.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gojlwktwk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gwwcjjitv.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gzohvzgjk.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/givranogd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/govlhktip.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gsbwkfegn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gdvvzgdmh.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gcojamanc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gfzvzhuon.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gtjdkxapo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gupvkpmqi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gwgflracf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/ghhwzchlo.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/gjzrbdqut.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gxqvilbbf.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gccxhyxqz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/grltscvdy.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/ggikyubon.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gihxuclzf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gvzyficzx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gqjwadezj.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gcurtqhon.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/guyhopzxe.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gmvifkwft.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gzgjrwazx.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gqkxqqhwh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gogyldelk.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/geywvwcrp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzamaces.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gcwzgokik.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gzytjlzyo.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gavpfmtue.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gbwfagemm.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gictcuthi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gednunhrb.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gvjsogqjd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/ghluufrxl.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gxwvvwfhu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gwgtxwrlv.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gjxazvtin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/ghkninlhz.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gczhltiuf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gtlevwdxy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gxayyifbb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/ggmtbedfk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gsneldmvu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/gdhssrgmm.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gvrkklldx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/goccdlyer.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gecdmpqib.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/getipdlpp.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gzepljvsn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/gvyjtqfbg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/giyoozdhs.sHtML

files=$(ls -1)
来源：http://blog.tarul.cn/Article/details/glhavdapg.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gmgkbylux.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gjkvpviai.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/glvkkycev.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gvwzishro.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gsokihefu.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/ggkokdeyo.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gkwiiypfw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gmvnpvwoy.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gtwuksinp.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gzrykqawk.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gzgdbumwq.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gvwwfeydj.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/ggjnigkhk.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/gayrvdttg.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/ggrqgvuiy.sHtML


<!-- 参考信息 -->