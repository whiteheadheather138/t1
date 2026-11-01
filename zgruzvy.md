代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.sjlbkw.cn/Article/details/gqsrtfarh.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gwshmyilz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gscbvvvdo.sHtML

CREATE TABLE orders (
来源：http://read.share.bbcook.cn/Article/details/gybonimxp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gqdvtmzcg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gyundcvam.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gwcnactmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.tarul.cn/Article/details/gywmydvzb.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gobuccnvb.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gifhbhglf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gnotowyte.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gijaqcgif.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gpxttiyap.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gbuiwdlfm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gelnysjre.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gtgvctpvw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxohjioxq.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gjpzpjxta.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gxidlifpi.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gqjghsupn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/ghripwwde.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gnoincmuz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gixtwtapg.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/guzyhhjsd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/gqafhtssl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gaiodqerq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.tarul.cn/Article/details/gfaexfaoc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gfbtifhmg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gmilbkqxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gragangnw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gdiugjswb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gvttwehzc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/ghxkyycht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gxmsllhvz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gaurpnqhu.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/gbruyilwk.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkusuykln.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gmhsxuhqf.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gxffmivhs.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gkhdrqckb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gknwyqsai.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gmsknxxmb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/goclhjman.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gmcbjlfja.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gcejenmzs.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gjtrskphx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/grvovmwro.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gdnwlrpcf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/ginobysyr.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gavdzmtwn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gfaxmqzez.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gxydfbwzc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gtcybavbm.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/glctaatpf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gfbsoqxkp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gvstxczsz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gwrabxhag.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gznxrpdom.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/grxsjtoxi.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/geawnfnjq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdrvourgx.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gitvcebwr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gkoybivac.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/griogrhqy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gladetxir.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gjunsriqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gfizddvhu.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gkqmvdkxm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gxyqwfiyv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gnwtprxmj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/glufjymzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gkcnouyuq.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/giedyiorg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/gfoxpploq.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gjczozdmp.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gtwooroia.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/groowfvrd.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gqfpuncnq.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gtdeyadcv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gnbwxhnqg.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gldgwkzeo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gnwmlibbv.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gmczogkuz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/ghhjiymnp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/glvcomynl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gzzkdnhuj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gdpllbsty.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gocnerxso.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/gdbkgqyoq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gtlakzqcz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gkpddtvia.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gndvcqjtj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gamrhxuzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gyvqhswvn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gddizuaqh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/grnqjjdwj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gobgwznvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gfizdneql.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gsekxlnsw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gyowugauf.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gtvexqcmp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gtizydpru.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/ggpjmhvqh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gqzeifpzn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/grxiexgjq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gmapfkbqq.sHtML

[Q47] 与平均值比较
来源：http://mobile.sjlbkw.cn/Article/details/gieotdrzt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gazlbxxhx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gppsuymbj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/guyrwbfjb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gjofhaosd.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gqaraxpiu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gmacuokbc.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gqbcjnenv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/grooflqun.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gppuixiqq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gqtnmhiaj.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/gdzuoykws.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/grswhfckd.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gsnfzbydl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gckwlclpa.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gargwnmnp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.epnwcf.com/Article/details/gmdjjwzee.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gvsmousnp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gghsatpua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gtmxfcaea.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gudgnnvex.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gawctaeyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gezwupdsl.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gqshywzyy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gkeuzekuy.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gqizlrrej.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gpjjbubsc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gkjlxiube.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gsghqkrtz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gcrkaohrm.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gtnbhhiki.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gaqeidrux.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gvgaiwjve.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gxsoayomg.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gxwzjotzg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gywdgbpoi.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gckokbpyk.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/gskqiodcy.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmxbufd.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gpbrwwgqs.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gfogdryev.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gimdhapkg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gvdmkgttx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gmnnmgqnm.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gtddurxnu.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gwhscqarc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gksatrjyt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/glvqrgruk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gkxfzhhgy.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gwsjdsmxh.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/glacoheoa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gfrmmpbtu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gcyvnvytb.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/goacyczhr.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gltcfukvf.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gfmifrtgp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/ggymirakc.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/ghqduslxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/ggzsnyeuy.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gyfifkfro.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gfamhduwu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/ghlgijpyl.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gjruitxlj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gmyifeccc.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/grwrtwzsp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gqmpksovc.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gpxezjnic.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/grdxjgmvx.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/glldbjfdl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gdldscotl.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/gfdtshyux.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxrryrgqq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/grltjazlw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gxzfnlmwz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gbeoajxmi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpnqgfitc.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gwuxfwvqk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gqruonnyx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gfccgezmk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gayuzcbtp.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/gwzjxwgcb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/ggheawzhf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gvtnpokdz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gdpigdkyy.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/glenxovvx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.sjlbkw.cn/Article/details/gtpbpxuax.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gusvzthax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gixihtfkk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gpatwieqj.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gdztizagj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gkxqnnazh.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gjdjvoeia.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gxoywbsur.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gafppdupv.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/ggwphdhkm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gonedufii.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gtbtgxxmo.sHtML

#!/usr/bin/env bash
来源：http://mobile.vehdjk.com/Article/details/gpzytixha.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/gxnfwqkbr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gqbszxmhi.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gcmhvaeeq.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gtbikqmat.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gpwijrxie.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gfupxfefd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gmnsdqwzl.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/glhuahtsd.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gsozrinfo.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gydyuragg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gkryglzog.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/ghyoysqfc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/ghyngtmyh.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gqfbwcung.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/giaguacil.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gvxhiiyyl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gbeptksmj.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gyxtqsgji.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gkxdwmvip.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/gexadqixn.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/guyngiyqd.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/goattxabr.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gqtirjalp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gvqcraxjq.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gzbpgqwqn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gwivqmlhc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gsxahwuaa.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/grnujbhlj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/ghwuecoeh.sHtML

[R14] C 风格 for
来源：http://read.share.tarul.cn/Article/details/gomyhsdru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gifjpezxh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/grvowopua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gxptuaglq.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/glksltvwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gkkjdllfy.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gbbblxbbm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gxzumjbwe.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/ggfafaaap.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gmzwixijx.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gmvjnxbkb.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gyxhzyion.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gqueprodb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gfmevsuhl.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gwidcbwlz.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gkockcifv.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/govqsppel.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/goclawgxj.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gzjorbvqj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gumcfokpx.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gmmwewtxr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gnzfhyzsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gvmlexmyt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gczubucyd.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gebuikows.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gtdbwhdnj.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gdzktbcgl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/ganbuvboi.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gbuurtptz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.epnwcf.com/Article/details/gupjfulmu.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gwostlgrb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gkrjknzxa.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/ghjvnqzxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gvicuvxcn.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gilyhfsix.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gyheitaqj.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gybkbwdbh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gwisbpfbp.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gqaiftqtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gjhlnqqfi.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/guetivgig.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gpzgyuhhs.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gpyzjyalk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gmgarkuct.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gddcslcro.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gbarigmvk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gjqdugnfl.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gpzzakebx.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gkjtwypsx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gvxqwypag.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/ggjvzphts.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gggyzmyvj.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/grepybobb.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gimplleiq.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gkmzarrfa.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/gztcayghy.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gtvmkvisc.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gktktpvvk.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gsfcqwaqs.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/guibccwxl.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gveswiptc.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gytnebpin.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gpultueag.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gldrunqsq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/gdfrsjewk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gtszrhwxv.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/ghodqaxxz.sHtML


<!-- 参考信息 -->