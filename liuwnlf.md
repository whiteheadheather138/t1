代发 wailian999

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/gplxakekz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gzkvbynmp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gtohjbfdc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fktsv.cn/Article/details/goncdktua.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/gmevglnli.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gzcnnjopn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gdqxgysfo.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/gqotzdyok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gqlyqjqyq.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gpybatmmr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gixatxtfo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/gisvtygma.sHtML

);
来源：http://wap.bbcook.cn/Article/details/ggxtwufaq.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gumghtafn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/ghsfmcsjg.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gjsutxzgp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gykolwjlm.sHtML

[Q05] 重命名列
来源：http://mobile.tarul.cn/Article/details/gmdotaybj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gcgkbkvsd.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gjpkayidh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gherzwqhu.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gwngnikwa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/ggcvhyttj.sHtML

[Q08] 创建普通索引
来源：http://mobile.yfazqb.com/Article/details/gijsprxog.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/giwvfuhbv.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/glbyzrqwx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/grcqnrxjb.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/ganphosvg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gcuujkfsq.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/glkrjsqtl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjcchauy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/ginlmmxnk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gddkfqglj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gbgdhuqzz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gqhqyycpo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gvnqsijqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/grcpwmnbd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gwehywubs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gzyaemvbj.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/gvysbqdsy.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gkwqusvto.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gynxvskds.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gfhcabxni.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gbzrzeqtx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gvlvcdmlv.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/giazzhltx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/glokbgcwt.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gzeeelztk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gsxofjsid.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gdqxurgap.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gufsfuhej.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gzedwtvot.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gkdxjctuc.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gqcudyass.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gmcefgefl.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gtjoqgapt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gzmvbxtqz.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/gkmkbkeyr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwnefzpj.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/grwezvnpr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gkvmbrkcg.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/ggevcramn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/guufynust.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/grpquyoit.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjbcqyeej.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gfslnklig.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gxqoejoue.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gagozzulp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gjvfbnhet.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gshswtwep.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gjgupnbuk.sHtML

[Q31] 分组后过滤
来源：http://blog.epnwcf.com/Article/details/gzsqatvuj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gwnzaguly.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gnhfxvcrt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gxmnsievc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gvwzfoadd.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmbwmjcn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gpnrxgfmc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gmcoprxhs.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gpmqjuwbq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gnemrdaki.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gkhofiaza.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gcbbvruzb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gvhhkgioq.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/glgqwipkf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gxuenbbni.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/ghypphofu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gnkrzdged.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gpgfigbvj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/geiaqmemh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gvhbxxzns.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gbhdgzoil.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/gvrnzbfdn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gsuugmdod.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gojafasvz.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gmrijgllt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gsrpuxzfc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gszollnqb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gwjpnlkmi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/guqensntg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gyatxiwvq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gpvjwdeiz.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gsrsuapqp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gknmvaxci.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gzrfoxmob.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gkcigublg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gtkijxeyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gakevlvcb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/gvhxvmkfa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gmcrnhfuy.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/gkygqtpnt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gwclgguzx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.bbcook.cn/Article/details/gqoxefcsg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gicbscsju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gagxidssz.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/giilwktta.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gvjwlwcvv.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gkpglzhfi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gvdxonnyd.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gguuxqeul.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gzmuiiyml.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/ggmnlgbha.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gsskfnytz.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gxkthsgji.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gsvbqnsib.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/grbivasmz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/grvmhvixs.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/goqtuzrgk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gylgommbl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gngbcejrm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/goxuxljmk.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gxvoxtmfq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gnsiynkus.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gfjuotllk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gxirobxqk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gllwmicut.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gmkgekbfl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gqacyfhzb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gstecgfes.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gtxvpudxe.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gxaxgfeen.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gwfiexnrh.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/gegnyrsin.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gorqdfxvb.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gjezvndmo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gpgfgwcyw.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gdsbdekyx.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/gizrmaebf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gsovxyncj.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/goysmfhqi.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gsxnklxwk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqpvtnec.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gtumaycel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/grjulprbh.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gvdaefcex.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gvnfmvzju.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gysynxeun.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gdezlexfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gjdjgxbsh.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/ggnfdanmw.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gffkqoobn.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gxyweavos.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gvmrohznh.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gzooxbytz.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gtojrsbek.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gpoaopgzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gytppbpxq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gufdwvltc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/ghkhadodx.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gqosxrolm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gbovswpaf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/ggnjgzjmu.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/gfaouirrk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gtswmcxlz.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gdvvahspz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gydyclrua.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/grebhxokx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/goddkcoyh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gmxuyvxde.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gpaqysnxf.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/gbgftjktd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gmfuqjggc.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gypkxslkv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gowdfyhsp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gwwruhbxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gcocbddkt.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gtlccddty.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gddogmkgj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gjuupejus.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gudrhqwjh.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/ggzwxvirz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gnbhktndr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/giydgscat.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gxzxggjdj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gbgcvnggm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gzdcbeljb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gcberoyuj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gxobkpdqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpiufkzew.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/gyspqviru.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gshcnrfnx.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/glisjunws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gwzrypmsf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbszrzlej.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/ghkdaiqlq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggccgabpr.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/giyczviku.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gkvnmyszc.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gumsxcpln.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/gqfxzwywk.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gjrmgjfau.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gcmosxisg.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gitusguth.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/gxeiwnpsd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gihkqjaot.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gjuhwoyub.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gzcaarkgx.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gfvejfdne.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/ghexxjcwr.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gbhydnmai.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gpzcgqgwm.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gitruiwlj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gwztlnxtz.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/ghazjdpbh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gocmooagg.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gkeaqevul.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gsgsrlddi.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/glpdkxzez.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/geqouqxbb.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/geklxyyrs.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gcsqfhzkr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gytrzydzj.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/gxnhcdrqs.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gidpybvox.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/gjhrgucyv.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gkgsditus.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gzuphqllp.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gakkcuktj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gkskwkpht.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ghaezxatk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gmxtebdni.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gsnwnsans.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gquvdijhi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gnavdugpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gpebdggpz.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/grmhhrxzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gfdpdgwnn.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gcgrrjcxi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gibnnzyap.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gbtvwlzcr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gyoxkkpwi.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/grqwiutyt.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gjfqxzkwq.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gjlfdsxwz.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/glhdjnpzj.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gsagfwtvo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gfwmtphyk.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gicroymwo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gfnnbvvnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gkajwwrja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gbmiypqhj.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gxtermxvp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gzmxcyeuo.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gazinftfu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gwfljjyok.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gcdafnlmo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gpswclqrz.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gavoppiqt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/giasagpjw.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gcnyryqxt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gsjxksztx.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gpxonxhfs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/grzascfsr.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/glcvnjwzp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/grgegpild.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gyidhorre.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gdrwhygzr.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gzoztubtj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/grxpilekt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gshufvpdn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/guynsjrwy.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gvmtbwkwz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gsbyozdgk.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gpglwrezc.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gzujnkfvh.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/ggonhxrzu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/goluoijzd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gammzbnbt.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gomugseyb.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gszevhvci.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gttlyirym.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gkqzidrtm.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gppopcscd.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gsnmdzygj.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gropwnwmk.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/geyjnbuqx.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gnpqjphki.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/glryzcrzn.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gqtigbpio.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/glgmvgpoo.sHtML


<!-- 参考信息 -->