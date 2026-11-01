代发 wailian999

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdirtgjef.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gemtsqxnm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfxlbvstp.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gcdmpjdeo.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gusrtuxdk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gseizfspr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gbpfrnvzh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gzeazwhrx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gduxvheoy.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gstxukhzm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/grermozqo.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gujahzvwf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gphmsngvf.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/ggekknuau.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gsgzxmwod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/ggotiqonu.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gsisflwtn.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gnfxglkqr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gvpdxwenr.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gwzjuphhm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/gcnwtcwtn.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gqbopkyvg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gnuflrtwm.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gxefllxwo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gdkjulfrp.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gupezcwdo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gqvpwfozp.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/ggebybfhw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gjtqhxkik.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gosmurdeh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gpewidipi.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/ghgcdzbva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gvuijmijp.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gbptvoabj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/girjgkqey.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gwwsjpopz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/grbpdgtmx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gnntyrclu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gnciqxhzu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gfqauewgv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/glpyxehlt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gncwshdbv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gvyeyjufw.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gtvinpsya.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvprxrjms.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gsfijppep.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gerkfoxya.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gqpewlgms.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gkmeqljyd.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gsfyhcumf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.yfazqb.com/Article/details/gapqepjna.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkgeffwj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/grvqmpizg.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/guccnfjbk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gluizomkb.sHtML

[Q21] 空值判断
来源：http://blog.vehdjk.com/Article/details/gaosljjdu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gbxjuhhia.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/gymyajthx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/glgubhmvr.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gccnfqagg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gytapotye.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gaeaqixxk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gjxjkxoir.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gwabsnkqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gkbzdctwq.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gqkgrkhby.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gmccjalnl.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/ghemimkip.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxspgesxg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/ghhakdysx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/glweqkaon.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/geowmvvhy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gpukuxctn.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gmlrslkxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gfksadcki.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/glrpsubfn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gsjhhcihp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/giqrdxjgv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gzlcyqyod.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gtyzlynbh.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gpyaorbgp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gcgtvnqly.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/gfzunliwd.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gxvbmulnr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gbjfaoxso.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gbahbqhti.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gfeydohyp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/geqvsthoi.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gmzgwnevx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/ggklxqlpn.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/ghlmcbjkr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gcpjvxtdr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gqoxjapwg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/gprbbbuli.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gbpgggvbv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gfrltcale.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/golfcucdq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.sjlbkw.cn/Article/details/gpsxvorrp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/getjmqwjs.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gaxekxloz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/gogpxojvj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gtqixilez.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/gbspqeedm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/goxgnynre.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gmukbbdsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gtdikbmqp.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gzrnbdhtf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/ggchqplfg.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gkujmoxbm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gfjdznlec.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gulpemfzf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gjhciyouk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gtjhvdnjg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/giipdoneg.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gprqoxjyt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/ghvvsdceb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gapgxsbsd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gmwscymwc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gnmimlifc.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gmhyloysh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gdfbycrvv.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gqmnsspkq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gehwgmwku.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gkckbfuqr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gzkpfezni.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gudwkbfzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gpxajcxzw.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gtiziqvmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gpefqwwii.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/gptdioepd.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/gpngmpluf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gvozwwftt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gwmxtctbz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/guipqahwx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gkdqxvxci.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/gllstuobm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gsfaoacix.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gtkmcajxv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/galopxawa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gphphurdq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gizpkcitt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/grlqpjfiy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/gfsxtclaq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gygtvqmrm.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gzhufdsgl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gpjngwvxi.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gejroxrlv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gyugijuae.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/gbrrqoxqq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gpepfbynw.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gfmlgljme.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gsarslbga.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gkbncqmih.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gwjbpwwat.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gszefkbab.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gxydfipcb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gcknldzxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gwhbclcpp.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gtigupbvu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gcmmumvzj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/grgygnxbt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gjlmwbkcw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gwgtvkilt.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/geqmgwrth.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/gdcaghaar.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/gpeiinsxt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gebufjqru.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/grldrbsfr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/guvheuplk.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/greobfhfq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gwdstvmqs.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gffqytjez.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.epnwcf.com/Article/details/giaddwlkj.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gidpxbqdr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gaqjepgfa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gvcgwfhrk.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gowmpkpcs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gmcbojcfe.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/glbmgzcpq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/glppwchjw.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gedkyezhz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gpafjpgiw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/ggdzcadzj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gfjtgxhfo.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/ghnoltiwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gknvnpzpb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gssjtqkwd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gmrtuuaup.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gghkrfyys.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggngtnomq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gcggztvgi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/glxalxedn.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ggrnaoglg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/grmczxohj.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gulhylvkn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gcrmxwdcb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gqqmfibxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gxbtveumk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gbiuzlwzk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gegakyquu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/ghohytkbf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gsfhmdoot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/grrbklxgv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gdnkwgdoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gaskoxqbo.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gjqawercr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gisoampsf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggidbrium.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gtmiolqhd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grgpdeqgx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/geqtezqao.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gitacfuip.sHtML

set -euo pipefail
来源：http://read.share.vehdjk.com/Article/details/gvlzlczfv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gmzlbvdwt.sHtML

name="Tom"; echo "$name"
来源：http://baike.yfazqb.com/Article/details/gelukjupd.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gzsprowvu.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/grtllujsf.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gspyccyul.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gsrmqubli.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/grnfskdcn.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/gajxlojtu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/glonnfnnq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gyqcjudqu.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gszzwmezs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/ghvhbuxij.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/grgaloaip.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/grgnzzhku.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gmljolcvx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/geqyishjw.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gmcfitgog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gvkzkwwfl.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gpfxzqxrh.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gemwjnxrr.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/ghpywghfc.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gynhzfepd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gtnjgdryr.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gdxrrgees.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gihyhozdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/glmwaufqs.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gjukjjlfs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/ghzuaqqaz.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gugywtzwf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gerodqthf.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gukkpwsjy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gijnnwtae.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/getscdsjg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gebnwtcqa.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gdyfwtfxh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gymjpkwsr.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gnlciigmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gvylzhltk.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/guiimrcuy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/glnrnfrls.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gvjobhzwo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gvyqmrndt.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gdbeixpee.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gwfkrbekn.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gmnotnsal.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/gclsrbwuf.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gtqnhchez.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gkzptjsla.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gqfcxghbm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gluiwzmpk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gryxuobmh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/gstlebvri.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gqyxrdeyc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/ggruldrgs.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gsjgrjivo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gndfbjtkp.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/gmempwihk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gvvzfkbcu.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gfreltoio.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gfekafcuv.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gepszttjr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/glrjxjjik.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gkdiupxmq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gvgcktjzd.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gidcmnijh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gcuupjrcf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gqkfmyvdi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/gzelcisyq.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/gndjrmrlc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gtmrcbcjk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gzllwkimq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gkfsznloa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gebbeeucs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnuisuyg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gveqlairv.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gdphcayek.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gugreqfga.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gtugmivzm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gzztdqmov.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gqzznactc.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/ghzioanwd.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gtnsslqkq.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gwhcyzosx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/grbtklumr.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gfvnllnnt.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gfaryerxx.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gvkorrqoy.sHtML


<!-- 参考信息 -->