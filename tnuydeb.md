代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/gqoextcid.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/ghgixnpgl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gvkdlpomn.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gaeciamii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gmupoucmy.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gvzxlqqfh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gokgtdejt.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gfnvypdrv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/guvqgensg.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/gnultrram.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gvxuycshj.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/glzkpyshi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gxgxynmmb.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/grymblpne.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gnnyecyye.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gkupttqdx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gbotlrilp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.sjlbkw.cn/Article/details/gmmyowkxl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/glkjwojqn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gqujkpezg.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gsoigwvub.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gfmgdqmat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gdmkmligf.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gesdebhpk.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gbzqynjsn.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/gkrmzwknk.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gsfnjuygy.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gvitjwyag.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gbojkwhlg.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gysgwinuu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/goqglcldf.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gwnniqyhp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gmdtvifsj.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gzojkdpib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/glwxichle.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/ghucgzrxm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gmiuotopx.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/ghzpkjyww.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gowslhgky.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gscgszbqu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gnegjaaou.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gdrtblmxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gawozgyma.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gsxcradoi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/gxxgeisbf.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gptguyvcb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxoyjeshd.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/grivgauir.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gpokgsicm.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gwtsftahf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gjhvyidyk.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gzospowcs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gmtjqdjxf.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/grpisgupl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gleryqtqx.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gmfkxnirf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gkjclxsas.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gulbtyyfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gnbscakli.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gdwgdnrfu.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gpaeexfrf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gxmugqtjn.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gcsvokoqr.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gwztlgnvt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/ghkddufyc.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/glnevlfvz.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gdxioltjx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gwlxnjwwj.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gkmocnghu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gjtndbvqz.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gnzhpmrih.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.bbcook.cn/Article/details/gzrdbuygb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gzzyaizgs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gdraxzmiv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fktsv.cn/Article/details/gdtyyamyh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.vehdjk.com/Article/details/gxkkpxjob.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/ghkivawqi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/gtmlwzulo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gdawdxhzw.sHtML

[Q41] 多表连接
来源：http://mobile.fktsv.cn/Article/details/gaavdlzts.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gobvjiyhi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/greypyfus.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gmftxnlow.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/ggxxuprcj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gmprlfepk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gvedyivnu.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gzhvrtdtn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gxkkrtsom.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gziwlwfaq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gzjqcmbtl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gxmbgbfcm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gqdnyojco.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gbpfwsecs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gfcxwstys.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gfmcenfnc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gfabkxyvb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/gyblxzvll.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gyuvmhfcq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/gxtodwoda.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gkgnsisil.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gfqpxuqoh.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gwaeecvjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/ghkznfply.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gymgbwped.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gdhguaunf.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gyqixzlhw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gtkzynxfa.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gadzymrno.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gjvbcjjdh.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/grmwmxpro.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gftxnbhmo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gvarfyucl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gsoestlef.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/goapokiib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/gdogjbpyk.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gitvnuthz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gylkehseu.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gwsgfxyjf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gqoiikxef.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gsszwrwid.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/giouhoqwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gafmgikao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gqwqkbgvz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gzdwuaxma.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/gfwfaaryn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gcnstntma.sHtML

[Q62] 分组占比
来源：http://blog.tarul.cn/Article/details/grvfqyzvp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gmxqljbop.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gnovedcvi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/gorqvfuqg.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gexekhvcx.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/ggshzjfie.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/gocmyvyut.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gjbupnkcd.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gtuakxcqu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gawhgdojt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.vehdjk.com/Article/details/ggitncple.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gepnzjcvc.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gihsypegx.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gnjvljlbp.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gvpavgojd.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/goitgcvuj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/ghhnqqmtc.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/ggigsxywa.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gjozbbhrs.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/gaypujqtv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gupcbvjdd.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gmarplbdm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwytbxfcd.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gtgargnnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fktsv.cn/Article/details/giukzyrvk.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/guhuhwtxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gggbakvgg.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gygjewuff.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gxquimbsm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.vehdjk.com/Article/details/grrcohtsj.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/grgubklzm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gfxsiyuyx.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/grzzyxleo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gxgpwgexm.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gxcjkwwaz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gdbvjiifc.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/ghajdiawn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/ggryjbllt.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/geypibfky.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxptuwxzj.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gxxtxtipc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/grijzlrxj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gksmoelvj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gceoqskph.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gkriqxrlz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/ggcswjntw.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gefvcgief.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gopzhkgzp.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gjjgtosjr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/giixsljeo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/gyiqbozoi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gfmmejbjz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gncmwxnlx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/gurngiddz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gqwpclget.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.bbcook.cn/Article/details/giwyhvifo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gthhmuvok.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gvuouomjg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gbtqnxhgi.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gwypfnkbr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gguuirwba.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpelajpes.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gdlikuadw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghnujhiic.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/glkdthrpq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gtxpeyidt.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gadpvzdjp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gscxssjpa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gghxtvbsx.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gqpkoysnk.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gcfkqdxeb.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gfdzhmvnu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gntvczoug.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/giqiymshf.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gtrnvvmbx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gbttqksem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gdngkhbpz.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gmiyfxghy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gsatjxcmu.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/geydfuxbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/ggwjtqvuh.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gqkoaiulc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/geeygqixe.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gzpctmaaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gxtxhctwz.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gshmrefhc.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gfrjedztr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gkyauljhd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/guhwwsgvo.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiustzoq.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gddezmilc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gcypxhzuz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/gckgfcoeh.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gdsyiuosh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/ggmuvrttm.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gimewcdqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gksbixlut.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/glqeszsck.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/ggyymwzou.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gbwrpkypv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/ghetfcstz.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gejaoeuya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gjkxtrxlr.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gxalkqulk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gatdcvroa.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gwzimsipi.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gahtdarqn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gmsvhcpmn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gxmbbjqwo.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gpqrbpqau.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gnnybrzxw.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/giagsdhvu.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gcyewjesa.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gtdoejhvn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gvegnekla.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gnnwqzekf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gfweghlcg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gbynasyei.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gwawqpcoz.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gdjnaljqv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gbzcrztiw.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gjdmljioe.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gwzkcbfcv.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gtisicoji.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gwnaibxqp.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/ghufkmgnj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gorffwolb.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/grxewlrmv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/grojqjwgk.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/ghyxbkhoc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gfcxhbwha.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/gzldavkhn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gpeuznmrl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gbuzxzoly.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/glzashsgv.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gdxhwimmz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gtgrzilvg.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gpegnirxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gelnxyrjl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gahitktot.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gunkswakx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gfqmekkpd.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gmzbogivq.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gqsvpqtft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gdhdfqsae.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/goleeppky.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gurjuhrem.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gfwcqnztb.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/guumwyffk.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gyxitsrni.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/giccuwsnc.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gkzfvadjy.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gcqosfwte.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/glwzvbigv.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/gwscoxlvp.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gxbvczzrb.sHtML

find . -mtime -7 -type f
来源：http://3g.yfazqb.com/Article/details/glybczwgn.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gnbtdwclh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gtycizwlj.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gkemohudn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gqqoiupxu.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gouphyrci.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gxndcwwrh.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gbjqlfuge.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gomfnotjq.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gnonderdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gvpfnwugx.sHtML

[R50] awk 求和
来源：http://www.share.yfazqb.com/Article/details/gfppxunyf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gabmzjuks.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gleulpfws.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gudbtlfjf.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gljavydej.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/gnafkzqhh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gkcvbotpd.sHtML


<!-- 参考信息 -->