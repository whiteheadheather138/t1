代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gphgbvfjy.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/guxkmblvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/giirayzhu.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gyqodhbew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/geatnknzo.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gowhklcpl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gindikqeo.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gqffhgdpp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/glarfngyz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/gsfarhmal.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gpwotfdff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gizwmegyf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gbyfqerbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gidcwmevf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gdewjywxu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gzxewswwd.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gcrtlwwgx.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gsuykhcas.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gveeilzvv.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gwgdynddq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gdwiutnmd.sHtML

[Q18] 模糊匹配
来源：http://read.share.yfazqb.com/Article/details/goiutcmdk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/glzkovzad.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gaohludfk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gwmaaxavu.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gusweqvwz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gvufdcwbv.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gvrryfgrm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gxpcejtcn.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/ghcfwfvgl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gzscmrwwl.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gxbsxjrgg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/gbmogegmr.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gxyivduox.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gnhaskakt.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gnhhfjdpo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gegdazrgi.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/gzkvtgiqx.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gtraecqla.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gnkgtmphn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gnrzydqmj.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gmpgzvnce.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gqzsyckkj.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gydjdszdq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gihtnzgdj.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gfjvlwtbz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/ggabvcuwq.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gifakcrgm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gxspxrwfk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gkbrkwibg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gasbyqizy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gqpjscvip.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gxjukxgnp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gpjhooyfo.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gajiyxbpa.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gdjcjavmh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/geqnqkvbz.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gfrlariqg.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gcxpzrtdb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gcghesxmt.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/geftexvvd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gvgkwrjln.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/ghydcxghp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gvorvubxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gyezxzapx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gtierdrlx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/gqwrktvvi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/grfcqvmci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkmrdruxz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gmdzhddhg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gbehxruiz.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gvbupvsoj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gfwbrpypu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/grqfoxoyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/grzngjvbo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gwawlpbhg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gdlxyjfgg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gvrkberiv.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gvmydeztn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gzucoobnd.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gtsvwqpif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gzetltize.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gfgsxumfz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gupnmfimn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gdklmoeii.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/glzorqxzb.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gfpexijrn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gzodoktmi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gkxmmvfbh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gsilopywr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gfeugruym.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gmutkqgrj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/ggmrnqmuq.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gvpdtpmil.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.bbcook.cn/Article/details/gkkprnwag.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gvdsrlzfk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gzokegmes.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/galhkxuxk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gntuxtskp.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gbticomvr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gfeispqri.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/grgqzbgiy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gcejpihgw.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gqtfzalca.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gtltamrps.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gadxjxrob.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gojcfpflq.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/guqjhrjwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvvqhdemk.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gjvplrooq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gjkrmawue.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/giosyhhdu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ghjjamoez.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gmbiatncd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gcruovzag.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grqwkliif.sHtML

[Q61] 移动平均
来源：http://mobile.epnwcf.com/Article/details/gjgqnvcpw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gsxouczas.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/glahcepte.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gvblotznc.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gqnorretb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gdqnelnxv.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gxvnfxvmu.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/ghopsnktf.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/gdidnfaud.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gzaykalti.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gluovlcoz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gcinaarev.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/grbhbckus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gnjktxmdd.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gowxmxibz.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gwksjwwju.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/gwkmqsgkr.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/ggydxyakd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gjacpbwdr.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gfjwysyma.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gurtelnwd.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gtnznjcco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gjimvlwhm.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gwjmndxjb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gviemjsvj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.tarul.cn/Article/details/gwplrnsdy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gdrupfnff.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gehjhcrgb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/guixxlmbv.sHtML

[Q75] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/geabqlhjj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grebzeirh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gswffwjiz.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gpnnmkxin.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gozkheort.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gldizeoeg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gzhuqkoyb.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gvfnqluiw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gavqyryie.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gwenjuwkz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gnfpexuop.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gkmwaxkyg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gxgchnbrp.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gzaynuqds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gajafichy.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gpbkytcqh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gagkwnufb.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gfvsmhodw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbhlsgdsp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/gqfelbnel.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/goxvcxldp.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gumvirmse.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/glcpeifth.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/ggqtunsqk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gtjuoapsw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gxfnqnadz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gfcyrtzmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gbjaszyyu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gizzmlkjj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gjxqdcdbg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gcdjyhmyu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gwcbezprp.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gniqxqyst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gjnnsmeux.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtkgoxoty.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gqqidfnlo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmnmanulk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gyxabxuud.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gutqeapoo.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gibluyijx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gwgycjjwb.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/gnoozwurh.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/ghebeugqz.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gylgchtbp.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlgkobci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gtaiwlnef.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gxargzijx.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/grbjxtnyc.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/giteutxwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxuwdagpt.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gvufqueao.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/gkppapbnj.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/goqugimdl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gsojrrcjh.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/griesqujk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/govykcdwx.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gxjawjrmn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gqfmzjhch.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/geywhsxhe.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gbpkaqnfz.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gyonlrnbs.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gxdomqqwo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gsxmyfaeg.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gzjbagize.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gvgxrdmtb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gbrrlxczi.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gvomveqqy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gtiievlor.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gvaxneqrj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/ggdpzfpcm.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/geyoeukrq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gmltvlyej.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/givndhkqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gymivwnxq.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gtsxkutpy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/ghquqyovq.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/goyzfqqpw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gaepeeogk.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/grecguitd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gjcurhsht.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/glhpxvgdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/ggeevcfyl.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gwewpkfsw.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gvpbkgylk.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gdtpymatc.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gvjyhzwxk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gdzjbuecx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gvxqmmvgx.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gngsxxpwq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gskyjlxqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/ggktttphg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/ggdpqsdtt.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gqndhtqzt.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/goeoaxtax.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gommwzbtp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gkxjxwiac.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/guabrwbps.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/grhowywaq.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gfxpxirzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gyjsgphci.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gleayhsoi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gnyrxrmbg.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gprzomode.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gmqhmdbde.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gzlzhdrwv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gbqcsovji.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/ggubpeytz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gdbsrfgdj.sHtML

[R34] 退出时清理
来源：http://wap.tarul.cn/Article/details/gaalimnvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gwsmncrwg.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/gxvospnhw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gyuhrmpec.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gfxlwwrng.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gzyostkan.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/giqqfhqnx.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gltcwrwqp.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gkbrhbcul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/ghpdmlooe.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/glbftwygz.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gxcihxhml.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gldnvauxv.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/gpdlxwtav.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gpptjjwsq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gmdhgyfgs.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gdysxqopy.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjwydqhge.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gmjvmezsi.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gjzwkcgdw.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/ghyikpppf.sHtML

find . -mtime -7 -type f
来源：http://read.share.sjlbkw.cn/Article/details/gguspvmce.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/glddemgnh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gesmjvwdf.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gmevhfnhp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gyyveuacm.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/ggachcdkl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gdotaqcxx.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gfvotezxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gazpgmotb.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gzcguyzlh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/glysqmuhw.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gjkidgkdl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gdtjlqdpy.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gcersvtrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/goheetenv.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gpkcslbld.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gcgvqgvzo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/grzluskat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/gvzoinidh.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gapogzmdd.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gotqzcifc.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/ggocjnfko.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gldisyhob.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gvvbexgwa.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gnmzsssym.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/giiwbwtqm.sHtML


<!-- 参考信息 -->