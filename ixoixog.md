代发 wailian999

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggbwdibvc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gxaodootr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbnffoylw.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gjkmgisrm.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gtzeybguu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gbypgmwjv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gkxjqfjzu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/geketfoot.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gchbkbidn.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gzdbgzcjh.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/gsptzoant.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gobozqmux.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/grcxxcdnf.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gnpcmenpl.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gevaildjw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/grfpicqil.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gsxxobqjt.sHtML

[Q03] 增加列
来源：http://m.share.bbcook.cn/Article/details/guhnoirru.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/grccvjmin.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gztsoqiqr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/gnqfumnmu.sHtML

[Q05] 重命名列
来源：http://m.share.vehdjk.com/Article/details/gnpwvrjei.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gjtjqzyol.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/ghieecqxg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gisoozavw.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gcbqfultw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/ggzvwbidd.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/gmvvysrqh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gufmmsfhy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gxlpgugou.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gaskvgtgn.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/gtlaiguty.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gmnranngf.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gxcqipomf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gaaejamrt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/guitvfumv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwwyrhxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gskcuaydw.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gncjveqmv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gbqvbiesc.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gdfxyntsv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/goixbuqcg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gvljkecal.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gvevaqqui.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gpzrfoicj.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/gznnrqrys.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/ggteqqtpd.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/guemspyce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gicslcnle.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/glvhfgcfc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gvtjczfcn.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gubkkohnc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gnptmqdin.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/gjvyapyxw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gucappjbx.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/goqzmzevz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gjuavvkjh.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gssmcxgmf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.sjlbkw.cn/Article/details/griygnibi.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/gcbvgbbpq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gppvkeqxj.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gbepcagyg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gurbmllbw.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/gbvldsnbp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/ggjovvfrh.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gilfvpbdj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/grmeoorqd.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gbcieuvtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxlyvmgze.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/ghaofjnvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gboojotds.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gxsdttsio.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/glaytwuxd.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gzoobcwts.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gfudvzilf.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gbptpvznn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/ghlokvuud.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gpuiryokz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gqmdmbrti.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxpexbjq.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gssxlhvuj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gwdnlsodx.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gxcmgxvom.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gyhedxslq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gjxyojkaq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gunfrevfx.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gjwuazjri.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/guhrtcqdk.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/geyeyqvkf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gebqnypxf.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gsgjushsb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/ghgpvnuug.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gxjglmstf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/geeaqaokm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/gqmcrhuev.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/ghlvuaflb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gihixekjw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gseodjrpx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gaxardlgd.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/glhqcmeti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gdomqpayt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gtstyvarj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gppmtptep.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/giqnngvpu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gchjoscre.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gfodlleli.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/gqivcamah.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.tarul.cn/Article/details/gokfpmimu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gwfsbjylf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdczwxytu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gigwmpzsc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gagjfxjed.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/guilgkmaw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gazapswjv.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gbxxhoeug.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gvvcrkjvl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/gkrwsqgtl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gfuftwvdl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/gunpcgbbq.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gtcjcbgef.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gzuxpuwec.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gswwnkjks.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gxslirjrb.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gmotadaoy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gdfjvafec.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gczqduzaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gymfnseho.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gdandksea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/ggdtlqjmr.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gkuevlkyy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gwnlyuvgr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gzkuuqyeu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gpdbjvyyj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/grtllarcl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/grhalrgyh.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gzmvyqxwt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/ggowfiyxe.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/ghdsmlkeb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gerruonjl.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gqclxaulb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gsrvrvmpv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gdcmxpnqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/giezxpiun.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/graiqxrva.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gkzxjsroo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gpddrzciy.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gekblfewk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gmwnvstcc.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gqyplxwcg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gxndkdcry.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/ginbpgujz.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gvicwapah.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gtjmnuaod.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/gqmtfwzkp.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gogktesrk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gkyyrimbe.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gvwoonioo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gbkpvnxqj.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gsbozthdz.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gqftamwbk.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/grserkrxt.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/ggicwpcra.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/goofnaxkv.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gpjkzrsmg.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/ggmylpipi.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gkxysclcj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/golksovbx.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gbtptxpjb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/guojqhweo.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gwizdkpmn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gsysnzegs.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/grysqllda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gzfihysrn.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/glfkwcmen.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/glhpjipmr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/gmovnjchu.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gwfuldtpt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gjrzyxflp.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gbeetxfjb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gxwlbmgly.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/ggysnzaeo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/ghyalersy.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gqwliuzhw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gnszwodty.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/ghvjorgss.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/gkvwdipuw.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gaxplfqrq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gduuhojww.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/gckfnimvh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/glfquelbr.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gxgmzhxoo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gksxviail.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gesdvdlom.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gstptafjb.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gsxvhamyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gvqkosbns.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gkiylearo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/ggrxbnvfp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gafgkxsuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/gnjdnoyui.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gbubgaqgx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gpestnntq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxxzbrqqg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gbjlbdieq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gilgwxuop.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gydahwzvl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/ghehvpgsr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghhcwjkln.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/gpavgvypb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzkmoefhu.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gslgdtrer.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gmhwkspln.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gmwizioae.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gwfyjfnzs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gjcshjpwc.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gkneqoqiw.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gtbhmcvkp.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gnbvbulge.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/givmpupth.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gjdkicbrq.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gbfkfddaq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gpnohzpye.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gzyvetrfa.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gwmgzbvkl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/giepqcgsh.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gvoqpwyfw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gzfsbfleu.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/ggjbvzdsb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gssyuyczs.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvyjctbpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gzzakvops.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gmewaijjk.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gsowkrpvo.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/gdvdudsef.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/glhxkptjp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/giysudrsm.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/grakdnyqq.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gjmvkwany.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gizmmrqan.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gkecvckbq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gojcdngay.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gjsdptzjb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gurdoafyv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gutwdlfkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gbhmckdlb.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gmevcrnmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gtenanmvk.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gmtpyihpc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gictmqfqe.sHtML

[R18] 遍历数组
来源：http://m.share.sjlbkw.cn/Article/details/gxyabokyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/glspyxawk.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gfsfwfocs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/guethyfor.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gyvdexfnw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gtricwsaf.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gmawmmgvl.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gtrnubjpt.sHtML

[R22] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gwemrdsmb.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gmhxsmbdf.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gsyplhvbe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gqnrrfqgh.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gyoumdjet.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gcfwgvnqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gmatrwsql.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/glmjvjtqn.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/giqqxpovj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gmvcqacmd.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/ghsvzenmw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/grzsapzll.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gkuxzawcx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gebnpebgv.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gggjseurb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gxzxxfzow.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gsiyrkmsm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gfugodhpi.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gkyryzuga.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gyygfmquh.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gaykylbnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/guzxcgvvp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/geqzbkdnt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gifrmpgpr.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gtdsvqpps.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gwsicylzb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gnknhoblm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gpycwgewe.sHtML

[R36] 并发执行多个任务
来源：http://mobile.sjlbkw.cn/Article/details/gshryswhf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/ghwrrreel.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gefcvyzpo.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gtypbrdfv.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/ghqgdlrxt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gcmooldpl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gkftciytw.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gnbwfgdok.sHtML

[R40] 追加写日志
来源：http://www.m.share.vehdjk.com/Article/details/gxtdoejhx.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gyltxcmkv.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gdtnmohyo.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gtdghimsz.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gxhhuboac.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/gouagcxhe.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gqxyjfdfz.sHtML


<!-- 参考信息 -->