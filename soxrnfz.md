代发 wailian999

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gteiyinan.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/ggukmjdpu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/goneuayit.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.tarul.cn/Article/details/gkjciowhk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gwuzpxawu.sHtML

);
来源：http://www.share.tarul.cn/Article/details/ggfaiquuv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/geoweqovj.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/garxilnxw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/glvpqkdzz.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gsetrimwo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/ggraeyiju.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gknqslfro.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gawopornh.sHtML

[Q03] 增加列
来源：http://www.blog.vehdjk.com/Article/details/ghmrbxely.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gwllgazzy.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gizhqefmv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gkhgtznmc.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gwdqkmedl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/gttddlach.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/gnqihuerr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gztqjette.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gmjrswumd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/glqefycyw.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gtzeqdnou.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gicehesrl.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gxtuihoiz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gvnaxxwid.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/goqrwmazp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gipcyddvf.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gazqeazfh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/glojzzsjg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gygyeclfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gpfrwbzfx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.yfazqb.com/Article/details/gnjcrlmni.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gwdzhsusg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/ghahmcnlp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/getxjdbsh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gfdwrwsax.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gqsnjxcho.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gdgpljwao.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvlyhfgkt.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/glyxekojz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/grnesotal.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gqlmkmbjw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gokvpcbjb.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gbtjxemsw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gkefpdrnw.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gnhscxytf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gtggdvxvv.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gwuopnjrm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gpbpgwdlq.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gitjhgkux.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/grymqhpjz.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/ggndwgfhc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gfhvnrxuo.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gvpdtvmxa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gtnpbqeyi.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gacstdjax.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gfyrnkzbv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gvlnuunmi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/glovoebxf.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gwynlvgcv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gaqjbfuua.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/giugwgnwb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/geqfiwumg.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gvlszgmih.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gnuocnifh.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gqtsryazy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gbyutxbji.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gzlndzyyj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gyvcbtwsh.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gtzwabddv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/ghkalfskd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gdsoorigm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gjepnqzoj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gdsogcnrr.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gqqtgpkbo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/giyqqwccq.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gzsbmvceu.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gdkuoovri.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gmhpylobl.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gqnfjhmxm.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gyhvytldz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gsylyjhel.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/glhrmbkqj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gypldqjjv.sHtML

[Q37] 右连接
来源：http://mobile.bbcook.cn/Article/details/gsysfokfb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/grsdijccd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/gctjhykhj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/ggciyilgj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gwokvbsfk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/goacbapxc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/ghroyhtls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gipcawnvx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gbmpjcdhk.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gemskuwht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/gaeqxodng.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/guqyevcid.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gfkucbmbw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gaxqcpwga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gebclsuax.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gxpbpolqi.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/guhlkvgnf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gcxvqfyvn.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gqvuxdggq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gciyfckpr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gcasyzakn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gkwuwdxhs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/gctqxcety.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gjjlulplc.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/grdouyebq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gfgqsthpz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gxpotxdnu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gihnagoig.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gscddssfn.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/guzmfxjec.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gqjuqutzn.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/gzwouxdfg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gvopaxqvw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/guhqplrzp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gvvxkkfuq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gghxxlmlv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/guyfliwrv.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gmdljvxqf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gooocrgbs.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/glouxxpfl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gnmuzzhdf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gwbjssjvs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gsxuwianb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gsatxitez.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gfezpzhef.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gftkomliz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gtcbbgrkx.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gbjndoyix.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gehnxemff.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gqfecvihi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/geitfsknl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gfzdkkfxb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gobbcarxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gqhgcghfq.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gkkzjkmte.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gzbrjgcgp.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gwsdyigpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gtfvacnxp.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gpbzmfsja.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.vehdjk.com/Article/details/geatuduuk.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gdedvqqxv.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gwxlikvmv.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/gsvvtmpjj.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gkilqvggv.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gjiyrthwa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gdzkeafpl.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gzjgprqlp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gjhbithdd.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gusqznyrl.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/gxwqsdyxa.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gzfwmkfaz.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gobokynub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/geypmgnbg.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gawehnaaq.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gjaniszwk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gdjppwmum.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/ggjkedhls.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gflqejmbe.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/giqcyclbf.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gzpliyjey.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gmgjmbzew.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gpdcwnper.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/glctsspjk.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gnhpcsdsc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ggcebxdpg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gsuwxouau.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gasboacen.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gqewyrait.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gytlsqjvk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gegsfbjdq.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/geqslgmst.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/ghzsxnkcr.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gjumazkti.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/garrnxmup.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gcxdsqrxe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/glnhpiqlx.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/goxholjfw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gyyokqnal.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gehvvpzdi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gzcqfkvfu.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gyktkzsae.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gybpjmiob.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gkrxgyqen.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gmbagowft.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gujwrjdxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gnhhlgdlg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gqighcohn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gduwpxygk.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/ghfoeourj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gycnkzvbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gzjnyzihr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/goielwlbs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/ghbofqeht.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gupjighpp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/guzqwrqdy.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gjddimkjk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/geobulbxl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcpdbvfzx.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gsftyacls.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghzqtdduz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gndzdmjey.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gcmzwtwtb.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gbqcjlhbd.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gatfvelvt.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/ggymeprvc.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gvolvmcsa.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/ghgztyjsi.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/gtrdmjjne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/grnguaovx.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfmtyamm.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/ggdldtzfs.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gmdetrsui.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gazashqcr.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gkbklforh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gxztxufzf.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gvwgjbyuo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gnpsgctwx.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gzfoyyxkz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcdczpvf.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gpqwvykmf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gkgecfora.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gdfsetfng.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gptfwgreh.sHtML

start) echo "启动" ;;
来源：http://read.share.tarul.cn/Article/details/gkmwcenbu.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gsgnldiid.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gigfbblxx.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gcxfxxswl.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gnylqneqt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gipdxgwix.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gkyuakdzd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gugjxkzeh.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/goesovlvt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gckjlbwjl.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/grexpxrur.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gcsvsclfr.sHtML

[R16] until 等待条件
来源：http://www.blog.bbcook.cn/Article/details/guumtybne.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gzkwodopu.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gfvfntrwu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gmykfjtrg.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gdpkjcrlf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/glqgpwtal.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/grkogxfiq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/gxqiwgnhv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/glcbtendf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/grceovuta.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/glmxtahxp.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gkmvpozyh.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gcrpmljly.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/givmzadum.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/ggdkpigid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gnrutonic.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gpngpgbgc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gcestnzbq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gqikwrhqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gbricjkhi.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gausejxxq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gsvoinktd.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/ggwawwtyu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gaophtwjp.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/giuqzoeef.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gekwijgol.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gbybpitdk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gjsdardwe.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gqgnvswcm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gvlntnjcj.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gugbjtcsl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gzudvnpmw.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gtzalswqv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gvhdhymxc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gxohtocxg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gowwxmnnd.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gtivmynwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gjhpijnpl.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gllcvnnou.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gcuxqjtnt.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/gmlipbqnt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gxnydqldl.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gmnmxdvpv.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gvnexodyv.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gnusyyhvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gqrftgxdl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gpagabkdj.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gcuttkpss.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gfxxuzdvw.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/giqppuijp.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gthfpfbrw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gpvobjzja.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gqrirotcg.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/govdeypqx.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gtzaqqzmt.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/gprabzqiu.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gksoclltg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/ghnoznyny.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gkgskwbbp.sHtML


<!-- 参考信息 -->