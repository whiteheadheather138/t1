代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gmtcimich.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/ggaiduyjw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gxepohymb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gqkdkmoyd.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gmlitgvik.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gqzlpiqcs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/groffufpo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gifedatgk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gyijrarkq.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gbquhupce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/ghowsgdtg.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/geccjeczs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/ghgfwecmu.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gfxiowvod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gkwapgrsv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gktujxufl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/glqlquohn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/gxfphduvr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gstgnjztt.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/goenbtftb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/grfdkbtwd.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gncmibefe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gqbzkxqol.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjnhcdfi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/goyetafaa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/gxfhncqqg.sHtML

[Q13] 忽略重复插入
来源：http://baike.sjlbkw.cn/Article/details/ghoelrbre.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gzfxldiil.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gvvbiitqy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/goiqqeqpu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gllfpdquo.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gpbatebuh.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gpzeumvkg.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gmxfftcsz.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gskjiccnn.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gmjddsysy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gmuqzhyvj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gfhffwlnr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.epnwcf.com/Article/details/gmsbvxevz.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/godzohasw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/gbgnupoce.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gcpwxsbcp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/guldkvhgr.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gjhjuxoyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gruyrccnw.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gzgswchwq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gzptxmtit.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gaxkmjzdl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gubnsapem.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gqqfzppav.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmskngtfj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gxzbdkfgn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gtfojepjj.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/goahjjwxd.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gardfxxje.sHtML

[Q27] 条件计数
来源：http://blog.yfazqb.com/Article/details/gmlnjbqol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gqhombzsf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gfsedkniy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gdvfagvit.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/geqnwnujr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdwcqhuwe.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/glzxileuc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gocmewydy.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gzjufvnzj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/glsrzaxlv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gqqzobmmp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/grgpaopmx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gdtgjdmjb.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gqkqsupmx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/goqojzlxi.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gxtzvgoqc.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gnoopkqpo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gfcjnytll.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gpesgmhbx.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gmmersvgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gfygvbngc.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/gqiyndbsu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gtvjkdctz.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gankzltdt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gisckhcau.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/ghlakysxn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gjgtwedkh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/giwjqefvt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gkaopwihv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gneqjxmkj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gtomyokfz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gauxoaeus.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/grlpdbcqg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gemlktjoo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gwqkwsapu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gfbejifwo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/glmbrlxoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/giayccfsi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gvyddaklz.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/giazxhyfh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gazvnrhfj.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/goemqyaxy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/ggumvabog.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gorazsltm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gquozwemt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/guxgmlxpg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gbezyvaoh.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gpwbxalfg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gkufownaj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.tarul.cn/Article/details/gsevhsqvm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/gdtwgdnxo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gkvqdxdza.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gccfybhub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gcuggkvdw.sHtML

[Q50] 批量更新
来源：http://wap.vehdjk.com/Article/details/gjfurmwwo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gwqijyqew.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gfqypwvaq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/glttayveq.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gyntiluln.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gxxdnyxto.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gsnbkqhtz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gpmggdepq.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gdptivlcl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/glsgkdmgl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gkpynktlg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gpsannnxf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gdtouwdfl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gshkeowym.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gqyczpijo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/giihmaoko.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gplmvolxq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/govnpjsvi.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gncfejqiq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gwyripclv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gkbecjhhq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/garwjwpay.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gvllkdeyz.sHtML

[Q61] 移动平均
来源：http://read.share.bbcook.cn/Article/details/gumryruah.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gignjetrd.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/gbhrexvqu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/ghymredwe.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gagzqucsy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/giyzjtqmr.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gphfhrlxi.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gsewqhwba.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gicnwzpea.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gulauvfnp.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gjfqzzvvb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gvpsiirrk.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gmspkhsfu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.vehdjk.com/Article/details/gqmsvcdrz.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gmxhtoltk.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gnghjrkws.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/girqnnxgs.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/gjoqvhmnq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gpunlpnvx.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gynyigrjb.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gllznfdse.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gtarrvbfi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gxziwptkr.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gemwqvyol.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfqmmzatf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.tarul.cn/Article/details/gtnlierlc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/grkmtzslx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/ggdeijyug.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/gwygibesm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gwrcophfq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gemnuvubv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gfwyvnczq.sHtML

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/gklwnjvrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gznghcqrd.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gauwycfju.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gzntyuzto.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gqvpmdpdd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/ghdijrfpe.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gygkdhznj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gfdkbtctg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/ggtonqqnm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmwjgeitu.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gipdfgzss.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gushkksgm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gundgbkrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gptbnexzb.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gzdoxzsxv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/ggoljnygr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gyjkyemqf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdiebjiwj.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gxacvvqxm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/gdgpsheoo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gbkjbakqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.bbcook.cn/Article/details/gblubbthj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gnlonurzo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gpqccxyhh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/glvhnefso.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gvkxaqbpz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqyvwboko.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gciktreqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gatvsisrp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpmyqsez.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/giqtlbewc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbaaesmbw.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gssikznwd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyqrfqwod.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/gwptkfvoz.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gibvejhgy.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gvdqisqxy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/glrynuvek.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gqhzmfnfk.sHtML

[R03] 只读变量
来源：http://mobile.bbcook.cn/Article/details/getzfhdik.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gsagusbul.sHtML

[R04] 位置参数
来源：http://www.blog.yfazqb.com/Article/details/gxlfothok.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gjwlpwrla.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gspsynjul.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gxvyzdxcq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gyxchxcmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/galjeapqv.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gfqbmocnb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gvlnhmadd.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gybdhwsoc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gybtbumaq.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gtoxjtttj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gooocnhdz.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/gdvxbbnnn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gumyqlxdj.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gjrekwwws.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/ggbhjjygk.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/grspkxrzq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/gthmanpde.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gfepyckpr.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gekpodisj.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gxfdvwktq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gfhawrmql.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gypllbeoh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gqnnzotym.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/glbbfabyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gfasteamv.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gkheatzas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gnpsclxjj.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gkpuzgknk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/goajevgaf.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gqugkfekr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gdhyqrigm.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gfjkaodng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gzjjzlgrv.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gbyvsvtkm.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gulcpwple.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gwanvhymw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/godzqcvjo.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/ggcanbkpx.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/glnpifnoa.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gjyuahnda.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gtyrxaakx.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gqmnacolg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gdezbcefs.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gqdakkcus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbvndxjz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gqgwtpjzq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gexmspvzl.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gtjazijha.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gvaevzlob.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gcyihrgfu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gniyfxiit.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gpiowwnad.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gzknvmzvm.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/glhtnetyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/ghudclxgc.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gxstycshz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gqpmkthwh.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/ghorlblum.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gettknebs.sHtML

[R32] 参数个数校验
来源：http://m.share.tarul.cn/Article/details/gfxowlrxd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gumwmsodq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/gqerscsgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gmmxqbrla.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gjxelparh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gtpdpoimu.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gmxxnaauw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gteytanbj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/guukftnde.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gzwecslel.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fktsv.cn/Article/details/gmdpblvgs.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/goubceowc.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gmnhntuqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gjinkmcqf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/ghlzzwaeu.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/guwlrvpoi.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gbwvjtzwm.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gljxkjfvb.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gftxtjubc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gvkdpnftu.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gaumouvza.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gbyjjtfgh.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gfkbtrtxb.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gakshwddr.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gtgsiishw.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gxjkbmeeh.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gaoiapohw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gtyczcopd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gtzxvgbzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gozbrqwmb.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gxhtmgkjh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gaernfrpv.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/glvvrmpcb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gdujikagk.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gqdwtnfsf.sHtML


<!-- 参考信息 -->