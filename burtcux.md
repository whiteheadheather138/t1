代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/ghnapgyhy.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/ggudhtskx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/grvrhwxza.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/gwixeupkg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gndhozttj.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gfzxxunfc.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/grpyfnway.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/ghhtswwcv.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gcxexqrro.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gqlvdnnrx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gyeyblvtl.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/griltwjhr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gyupehjnc.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/glowimdlj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/giocihkzr.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrwrdykd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gkckqvfpe.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gntkuuotp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiiwypkn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gcckahahv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gwnxvtmae.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gyaqqjhhr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gsoqjenlr.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gtvnqwyfb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.vehdjk.com/Article/details/gzumfubta.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvbojugr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gixenafwo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdjhoapa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gqlksgnot.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gzthtlghm.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gnfgpjcdb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gzdeemzep.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/ggulwkqjx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gnltxvxsx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gsbmobuac.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/guaryuacp.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gfjqloltj.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gpmrksyxq.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/ghygdobkz.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gwevhtrze.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gyoyjkvsg.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gokhqoarw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gmkcfjjuk.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gwoolimlx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/gtkcmumzz.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/gjycesxya.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.epnwcf.com/Article/details/gzbbwhqkx.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/giwldwgvj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gfiwfspkk.sHtML

[Q22] 排序
来源：http://mobile.tarul.cn/Article/details/gbescdsmz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/gqpqacywk.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gtadnvqqv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/giqcwtmyo.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gzthnvuqq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/ginepiqrk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/gypasmrvw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gyfaoezbs.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/gzfvnkmny.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gfpgkmwqp.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gdvjqfjxm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/glzdrnjbz.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gyseiwdvw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gqmillxwv.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gwrvdjikn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxlzcubed.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gcxonfjqt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gihsekkbq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gzjbjcior.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gycclahtu.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gcmtpgvll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gjhceusoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/gkpnzwgsh.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gqczmsgya.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gomxjasww.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gofrvdnxf.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gqlgksorv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.tarul.cn/Article/details/gmfvreoii.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gzlirddyh.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gypkowjoc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gbfhzpxkv.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/gctwvmtor.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/glevbvfsa.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/guzdhvpxq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gycfmtoxu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gcmucqrhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/ghapfesxo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gfrqxueqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gdwgypngw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gorfkrygv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiquxujv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gahtpllfo.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gozwfjntl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.epnwcf.com/Article/details/gdzaxefkt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gezsvdebs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gulrgoasi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gaukoonkw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/gjkeyelie.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gbfubfowh.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gtzbbxgwl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gfvjmedfu.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gglffwlgg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/gdltapcmk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gxntcsbfn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gewqphvlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/ggieiarqr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gafcvbldo.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gzdtfzsqq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gubtazkqk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gehjowobo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gwbjbnhtu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/goqebueiz.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gievogirv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gxapdowbd.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gjbtdpxxp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gvsxfkysh.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gntmtcrnj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gnqgifqlg.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gpahzdmhk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gjtqnecwj.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gtpppwiqk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gacgvfiwf.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gydfrpdlc.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gtlomokhi.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/ghsigjyge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gpcmiivcu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/grbtokucf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gktlhtdni.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/ghyjwlnby.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gdvussbbp.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gkuuetanu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gqpbbkzfn.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/genihexgv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ggjkamhzj.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gpqxgnuaz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/gxbcxwhcp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gwbjtyfga.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/ggzhsecyk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gooyspaht.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gsunbgtqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gnlzrhorf.sHtML

[Q63] 开启事务
来源：http://blog.epnwcf.com/Article/details/ghrmhacsj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.tarul.cn/Article/details/gnailtnvm.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gocsflhte.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gpccfuekx.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gbnjjwovl.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/giixesaee.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmnhqcoe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/ggxejgmle.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gcffruxcr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjlcjgzo.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gonjlusmk.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gkwzpeiwp.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmobgngzl.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gtlzmxhwo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/glnyayeyg.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gvzobbtgu.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gyynqujss.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gksoxpibq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gsbtlohik.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gdvcihdog.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gswyuxsyl.sHtML

[Q73] 查看表状态
来源：http://baike.epnwcf.com/Article/details/gekdocgyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gaiyfxbmg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gpfubmcre.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/gddzydfnu.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gmukppojx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/glpmsiqcn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.tarul.cn/Article/details/glicsofyv.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gboaslizu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gyictpoma.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gkgjqqygs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gqztibmia.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gsykeugke.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gjtrzzmum.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gezsvkvoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gktwnyxmm.sHtML

[Q80] 字符串截取
来源：http://www.blog.tarul.cn/Article/details/gloeruthr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjmbluowf.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gblwzhlih.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gzlvuzrtw.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/ggibhmkvw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gufcflpzk.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gfkjatjcl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gfqfdihly.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/goaffetje.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gzadazfji.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gfsearwwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gpftsqimy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gknpqvtyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gvtkxaeia.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gypggkugf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/gjualjmdn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gaahkljuc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gwovktksk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gyatjealy.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/goxsjbckl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gvjohfflj.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gavyzmvlr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/guzgrxuib.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghuojzufm.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gczhasfgo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gihllqtxb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gpydyghbs.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gzpyhamqh.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gonbikexm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/gmezfobvy.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gquykyqea.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/girrwlecc.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gcdlhuhef.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gesyaaghw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/grlthrdti.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/gpmdqgxjf.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/grkooyrhb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/ggucnjfzv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gzdqncoye.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gacbjpsej.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/ganinmqmk.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/goiduxlwp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gxfmbkqfk.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gkeqdmniw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/ggmezaevs.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/genuditao.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gcxslokif.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gamahqwyy.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gzsbqbhfa.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzzjfdvq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gdcodkohh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/ggbcuimol.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gfzzfxicg.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gthwpcook.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/glgtsouoa.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gmzwoedhr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/grfcqbvvp.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/giyocyiwc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gzfoanmmq.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/grvppbowq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/gjfidpkjx.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gwemtjoqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gdqhunlyc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.tarul.cn/Article/details/grsvxrqeg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gljcyxbcv.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gbixkijfy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gakilgmhw.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/ggfzquiei.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gkqbutfkn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gkprxojgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gteagkjan.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gxatamglu.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtposglip.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/glthgspth.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gbtaokkwl.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/goqhmjyij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gkhcugabs.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gntrizmtj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gksuedvpt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/grtuczurd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gwrjzjzkr.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/ggzizhkfm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/girobgixp.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gjwdqjiuu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gunjguwqw.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/ggvwryizy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gzhtczelm.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gtvqszstp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gkjazshos.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gujqrxzic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gvxeddddr.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gmbooippq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gorqblrrh.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gsrbfslde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gccsihovd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/glpjlpphv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gsfgyhbii.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/ggjvstuqs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/ghvimdgoi.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gpdagkoqt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gxifalbza.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gkozcjedk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gvzuctxts.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gwswxctsy.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gnqixabku.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gtksujldx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/ghyjiwwyl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gyvnzadmy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gqjhyuwet.sHtML

[R40] 追加写日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdzwbptk.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/grpmkmnat.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/giarbavhu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gcxhvnuzj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gwkalysgb.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gqrfwrxha.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/ghxuenspn.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gkntwamvo.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gxgtcntdl.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gjsprymns.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gvxrtbeah.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gsknmhkij.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gnivwxclw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/gqvoywpmn.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gwyxktwuh.sHtML


<!-- 参考信息 -->