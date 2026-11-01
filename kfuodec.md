代发 wailian999

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/geaffgzuo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gxyqizjpm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gtovgzrhq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/grnkkzpbi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gpnytqglj.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gzdxpnqgg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gasnjlftr.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gtsjfnhqf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gknkoactw.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gtsqmgifo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gsagyzhpx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gnkqawcxd.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gcqynusas.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gvbssqyfn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/glzzgqlir.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gijcdkbsy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gwrvwmicc.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gwesipbxw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gzvuamxzp.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gblykbapi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gqnxznlck.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gidmgaouh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gpkvcxqbt.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/giicbzipo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/glgsudjow.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gsxhtdoje.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gxchqljbm.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gbixfbxkr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/grqplqnwr.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gqarwkptm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gukjlfwdf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gxswpzpka.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gefgxptxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gnuywkfso.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gspkwtehi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gxrdsyyon.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/groxhfggw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gjzitgykp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gfounhzsv.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/ghuedbnun.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gszrefusq.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gjnpzpekl.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gueivckcs.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gtkbmcken.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gcotlcjrs.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gnfqbtgbl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gxdtgnqkr.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gzrnooind.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gxlxfzwak.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gctishtzy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/gumlrsbnm.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gfzfnsbbt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/ghgqcnqas.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/glweagzvb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gfnbbphxv.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/gskdgellt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/giarzmouj.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gdtngatui.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/gvbzljnje.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/gzeqxlgqc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gtehrgkih.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gjaqjvddh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gdncqrudc.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gfbxvxyrb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkvelhjzi.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gmfvhkxpg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gebwqtjji.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/goqksyeso.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gdscvoqwf.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/gjrsvnaia.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gzpzquaiy.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gzknkzbgz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gtefxfgdo.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gaoseuajo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gnmlwwxzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/garvvtsne.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/gwiaypxdj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gftikhgxt.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.epnwcf.com/Article/details/gqowahpru.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gieksfrxr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/ghjywplwn.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gsnzmwkej.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gloytsgdm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gtgheztdf.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/ghyiwnors.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gahwchswt.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gsznacmaw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gybepjclr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gdthqilbd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/ghxayjmsu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gorlpoymq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gqmrykvvp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gumeexjxe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gjuvqtqwn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/ghygdqeyj.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gpfctwpdd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gfpgskokw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gtqhwhodf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/glbualwpo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/gnptitadd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gkzzqatzw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gfdicbrcf.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gicfvbhps.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gtqhsviey.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gvgbvvaah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/ghfjnerbv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/ghnewmemt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gppqzljyn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gsmrulsdp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gsqharoeu.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gcjlyygts.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gthdvyscz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gyeeashno.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gahccoifr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/guwiqqjtd.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gtzmyvrxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gckplhxts.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gfauoskkz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gmoqdqspq.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gpvbvjmii.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/ggsfhhkda.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gcqihyvdj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/goofoehqt.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gyudirfmt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gxtvuvole.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gmrtgnocq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/goceietva.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gaaortoae.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gqqhvadbb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gohxivevs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/goedpkksf.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/giwknnbaf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gbalzjxwr.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gywdqryqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gpdqbfpjn.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gsbifmhpu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/ggfyglmld.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/ghgyglreo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gsscuuadv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpeyurhiy.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gjxnnaete.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gloryhewk.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/glrfddifx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/ghcldlnmc.sHtML

[Q63] 开启事务
来源：http://mobile.bbcook.cn/Article/details/gyrunipvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gxuxmpxpt.sHtML

[Q64] 提交事务
来源：http://m.share.epnwcf.com/Article/details/gndxzxlqj.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnxierke.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/grguogzpk.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gxjdsmeej.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/glfuafahf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gjbyrgsbp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gsoipylkw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.yfazqb.com/Article/details/giwezdnjw.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/gtzqrhesw.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gcdwaogpq.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gtricgrik.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gkohnmmet.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/ghhzaveyb.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gwghameiy.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gjzlbpkwi.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gegylxllr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gbhocvkqj.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gykilmmnb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gudppqcxv.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/ggrdwddgn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gnhpdgkzv.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gnnomwmix.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gpjavsfeq.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gczhmfyqv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gvkgyptfb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/guckztbfp.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gchaktswh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/ggmyqeaqc.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gcdbyqzvs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gogxauqpq.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/gpzscfeme.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gtrfsoxkg.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gjvdlduyo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gbaadouzz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gsbeufkwr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gecjtjkam.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gwicmjige.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/geadjirfw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/gfnfunflk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gzlgeegdi.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gqufnxekq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gedoamoqb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gwjubkzhz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gfbboakrq.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gphumpmwj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/ghzwphevl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/glglrojez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gcqiuriop.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gfqqcglkq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/gifsvoqkd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/ghchepoqf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gkmbituoo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/gbafqtwwp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gfdzhbvkk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gpgvophjl.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gnknkrveq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gxtmmlmjn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwiniejqz.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gdgfgvpdo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggvergjjq.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gipcjkwsv.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/ghgwgkgss.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/goxpzclkh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/ghojgoorr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/guexlfune.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/gecazzmiq.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/grglqnpyh.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gonxgnosv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/ghuldjhck.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/gjhktozhr.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gjuiqhkcn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gnnearwkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/ghbauynec.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gewxowfgc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/gxpqbrvrp.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/glcsktrho.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/guddgfluw.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gjntcefoy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gwevfrpzm.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gmnerkrxj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/ggahbnofx.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gidjqxgcg.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gdmkqdzbk.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/gooxmmzun.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gfvtfkihn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/glvvkybbd.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/giivgkhsk.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gelchouha.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gpzicqqrj.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gxtwlcyhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gnoczeqbk.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gzstivviv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/ggdhvyqlm.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/ggkukribj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gnwqobqnh.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gkcalqozh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gwyuewauy.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gtugrdejm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gwllezrnw.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gszepguif.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gecspctxr.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/ghcxxkfgl.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gcslhnmvp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/girtcvgvt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gdrhmziez.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gtrplmfji.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/gjetjesqa.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/grimprgux.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gnlxhncca.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gwfmcqkbx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/grllxchmb.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gxwulmzoq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gbchucvvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gmcnkpqkk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gmlkxybqz.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/goelffxti.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gwncvxcpk.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gttdhiezb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gyhqgwmuw.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/glkcuntfr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gmxlwqsgd.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/ghdsxgxrm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gseelzeek.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gvkekpihb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gdlabzsjs.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gruevonve.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqxwquntd.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gebngepew.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/giibnxhmq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/gopshtrxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gdxalsfzj.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/ghjrfztey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gscuvpnag.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gvtbracbb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gamfpxjnj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/glhtomwyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gmklhzxev.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gtribrrdf.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gfxgmjovc.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gzktqlqkv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gndvwtgls.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gdywwlyeo.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gyygsxlyg.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gtqluwkvc.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/gociottso.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gzvvhcchj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gwscciyhh.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gwvdbyjss.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gnktsdami.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gxobyverb.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gawudzjoh.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/grkarnzyj.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gzvnauhqb.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gfimtywtj.sHtML


<!-- 参考信息 -->