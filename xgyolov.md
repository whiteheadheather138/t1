代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gozyowxsr.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gzwphzqay.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gsjoryszg.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/genyjagqw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gkllflghv.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gjkgsfkja.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gcvdtbljl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gbmehiyyn.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/ggtocbush.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gamssmqyp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gdzqhbktv.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gartbnvuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/grgjcibpm.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gqfhgplji.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/ghjhauipj.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gfywqxumy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gocbhbtrz.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/gftmcigyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/goqeiotyl.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/graahznrv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gcdypqeuu.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/gfcttmjft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/goaytqbsw.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/guolgolsj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gpyrpcqum.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gbhzverxq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gcnkpemym.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gdtbvkbwe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/galnonvlr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/gwhncylbx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gojnmzbjp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gilyaarze.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/ghmwuplhw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gsezyecxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gxdxumnxv.sHtML

[Q15] 查询全部
来源：http://blog.vehdjk.com/Article/details/gbqtvumwi.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkvxzujjw.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gnesmphux.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/goauqlwoy.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gvgnpcnjh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/ggjbgmsyr.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gonxvedea.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gkuzucvwh.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gqvfgqrbr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gjfpdtkvx.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gqarkeiik.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gklyjyugl.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gvujsefzk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gmxqbvorq.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaettacn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.bbcook.cn/Article/details/gsvgcivth.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gqenclzam.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gygnvalyo.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gzbpjtgwz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfsabklzs.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/gbzweijmg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gpzoldshs.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdswdxas.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gdbtynztt.sHtML

[Q27] 条件计数
来源：http://read.share.bbcook.cn/Article/details/glvemnjhx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/ganeyuzgc.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gledqpovw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/goxvcqzkp.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gcrmvmtwa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gxqmwwioi.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gfcveskki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gasoymmmn.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/guhotinwj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gquqbbgmu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gkovccspn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gtfgubpgl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/grtfwsahn.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/ghdraorta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gwavtvsmn.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.epnwcf.com/Article/details/gvljwurrk.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gkfudozrj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gbewxhlsh.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gomypzdmk.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gwhnlgxnc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gfhbhatac.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gcrinsidw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gkfgbzdei.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gnrbgzbvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gvmrtcojp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/glvzavypi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gjtcrthra.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/glwunlavx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gppqcglwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/goibrfvcv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gtnavital.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gmegufojv.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/gpbyhmisa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gnnheyqaz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gddxpjccr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gluppitdb.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/ghlnyjzyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/ggkbjagvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/grulcgtyg.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gxzgzcalj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gcurbrbmc.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gngwkqaaq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/ghxomzymx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gtsbwtlwl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gplbpjcdi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gggfyhdkp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gdebumvrt.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gamjxyjia.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/govbcmsio.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gmwegmhgd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/guqzyolec.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gmudzubdl.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gosvuqvgw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gvpfsyiid.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/ghvjxnveb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gfnvkybhc.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gdgypwtpa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gxmwaftca.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gifekfywy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/ggraqkkfl.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gpjtzuxls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gqvupdkml.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gpfvtauxy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gahlxaznn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gqwckhppq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gbndktxvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/grukvzler.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gttpykcfu.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gwotrilmn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gibjwweno.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/ghurhzngh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gakqeslyg.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/giewjrbsb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gcmssjzsz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gxxmqkrjm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.bbcook.cn/Article/details/gaffyggfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gqimujezo.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gwdwceied.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/grjhcmccq.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gttlakxns.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gbgvxrnqv.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gcsvpjgbg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gaoqijzmd.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gsoehkgmh.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/giuoajqge.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gecxrkhyg.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/ggssexmyf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gdrooesmk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gqyeqciqv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gsbpcshnd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gbebwhjdy.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/ggfjyqdva.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gjmxqrqqb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gfrbaqhvp.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gfquhwmcc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.bbcook.cn/Article/details/gljsvdibq.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gjrfjculi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gdtmcdaer.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gwjxoizdv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gsbbqbcih.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gayzuokev.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/gngumbxdr.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gicqsakre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gthgteowj.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gxjloyppa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/guoladdsy.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gkzqudhrz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gftkuplxo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gmizzdtuk.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gblfpwxyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gwyhsfdtc.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gvbblbctn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gamwudqyo.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gqqwvgbqt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/giepbsdob.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gevhwlrnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjoufeam.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/ggskkhltl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gddrisjxy.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gswumblzk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gqyshpnbm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/glezdfcam.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjwknbrcu.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gzpkoshsy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/grukizwfl.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gbvpgllpf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqneujxzz.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gpdxeyyss.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/glvfbiazb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gzzzrgydb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gdddaedhl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/grewvjase.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/grzkjescp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/guvovtjwp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/geiinatez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gzmrinxnd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/grfnmaule.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gncmasnze.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/giyntbphc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gxsgdmnkv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gknwbkvrz.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gppltlspb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqggqpagp.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gogenzppg.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gemedqssl.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gsfznyets.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjbkcxig.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gqsfduyig.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gebfwbaie.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gmwrbbrox.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gahcbqlfe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gzzrrwljl.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gkunijqdf.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/grsmkhjrf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gesuitpoe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gkighdmwk.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gbqzcstuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gmkdumfhe.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gisugelwm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/grngwzfbd.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gwtrohzrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/ginqleouu.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gjzgxzief.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gajpniwtn.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gcfiwchmy.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gticaxoma.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gvsipuaxu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gldoqaphb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/gjzysjqxi.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/grwdgdgai.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gtappgcks.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/grshtxqgr.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gcvcomwqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gpobtaear.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gmtyiyqgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gdxbcsdzk.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gztdwwtzs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/glkslbybr.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gmvtdadxz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gfwpvoume.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gjpsrlgwh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gwzugjhny.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/ggzbehxff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gllatdlyv.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/glnqbzlgp.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gxxcgzixq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gtbzhmgef.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gllumlwtt.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gzsfxrpct.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/gjogwpvrj.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gebknzubo.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gitkahzup.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gcjbeftuw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gcwgcliav.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gfrdzctlz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/ghqwqjwar.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gtmqmqkoe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gbethgyjf.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gdehdrqun.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gspxchiks.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/greajnwjo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gzwishwts.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gqajyrino.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gtuafmuxf.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gghxcutqt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gdpqujbgj.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gtkoirbgz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gwwpicvsi.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gwpzvbncp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gtyoqhikg.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gakzpieyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gzetftqhq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gqklzxzqh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gdtztxqsd.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/ghkceqnpt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/giwymyear.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/guvefznyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gdgfdziud.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gewbqagrb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gljveqdmr.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gmmcjvlhb.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyozbwog.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/glsrzgurm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gssxjyqve.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gdeejnpiy.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/guhqejihd.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gkcouvrrk.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gkfnuhvng.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/grgbksumz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gszfvwewh.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gmehxibkv.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/ggmqrloyl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gvuguwsnh.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gpifxsuvv.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gztuytylt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/gjswhiikl.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gcpafdcqc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gdnmrvenx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gnthwfqoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/garnkdqmv.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/ggaorvwpp.sHtML


<!-- 参考信息 -->