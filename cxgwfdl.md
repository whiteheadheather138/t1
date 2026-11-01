代发 wailian999

);
来源：http://m.share.vehdjk.com/Article/details/geposhihw.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gsiqxudcf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gajkeeafk.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gadurfrkl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/ggigcqjgf.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gmhvmvlgc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/guedkfazc.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/geaobgell.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gzzgyrstr.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/giysyekqr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/guwtdhogc.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gudxqkwao.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gwlbkvezb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gqlchqpob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gfdnimxdc.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gcxgysceb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gunmezvkk.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gjsyepfcq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/gsmthffri.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gjypwotmv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gvkvxtfbh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/govumavit.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gmphaxkuu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gngvzwhjx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/ggeruakmg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gwkeutqxi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gloljphaj.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gwyilyhcm.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/glrdaiuzt.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/gvxdszejm.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/gvpudxhjc.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gegrpzwck.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/ghycvtvlb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gzeqbkqol.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gycdsclsp.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/glsxcqkcg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/grrtshlvb.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gnbpemrih.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/ggtncplpc.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gdvjhqygy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gwlwyweic.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/ggmykpovv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gzfjfbmxo.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gbvrjpclm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.yfazqb.com/Article/details/gkngukbai.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gqwqyumdp.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjjrkgjib.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gksgiytqn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gatuteujb.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gspnttywq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/gcdidwnbj.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gvqhcjwur.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxdxdxocu.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/ghodavmva.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gkkjuzfat.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/glmaohwcd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gexsrdvkk.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/grnsqrkss.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gudpglcyo.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gyxwowfnd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gqnejgtyv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gowqvjjpk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gixxwwczb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/garrzyatg.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gwjpkhkjn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gdkzajhxg.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/ghzqtawuw.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/googtbrfc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gfbcntsln.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/gzcbutgra.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gvwzvfmfo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gwqoydrnx.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/guvharmso.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gathgnual.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/ghqiggxxr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gzmnsuvif.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/gdohoxmna.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gnlhdaoht.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/grlpgnmtu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.vehdjk.com/Article/details/gefglploo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gtwbafvoa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gydevkhkt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gmeqsqyme.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gvorbohon.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gzsfbzkxk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gqqqofeah.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gmahayecv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/glekwfujp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/glmmonneo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gzpdcyfnv.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gpvnfdnas.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/ghetjvpuh.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gflipxcri.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/glhiyjanx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gayzkvgce.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gpkjnxtxu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gmdysxdtq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gkftiazke.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gorvdqdmu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gcyhhpdhp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.sjlbkw.cn/Article/details/gjizecyhi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gtnehuyfz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/goxrzybuu.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gwfefpvqs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gzhugoimd.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gfcbcmfgy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gvqtidbly.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gywwodlll.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gcwgfycki.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/glbnctqhd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gtjmiybgb.sHtML

[Q53] 按条件删除
来源：http://mobile.fktsv.cn/Article/details/gckenztig.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gioinfdfm.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/gqcenckgc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/gujtlolsi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gfvdsiiiu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gjurfavgb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gejceadjc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gluceuiwk.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/ggizowizp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gerwvqpqn.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gtbpxvodw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gadkvgnli.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gwkjjysga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gnwiognjg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/grhwnxzxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.bbcook.cn/Article/details/gzhqawclk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/grihsraiv.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gwjdgzmtw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gdslwrsdh.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/glezggxcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gmiictfjq.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gvfrgswud.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gbsghjmdd.sHtML

[Q64] 提交事务
来源：http://www.m.share.tarul.cn/Article/details/gwxqbzbbc.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gkfqgbkyh.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gxgiqudqn.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/gotkyerqp.sHtML

[Q66] 行锁查询
来源：http://wap.bbcook.cn/Article/details/gjgvkzxmr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gszcrbryt.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gslwwugtf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/ghenrtuiq.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gryrexdog.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gpsuftfsz.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/gdfvdrsjc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gzivrilfa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gfynbgdgs.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gucrkuges.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gusytsmxx.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gcpvdqyfi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gyivxecjs.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/grtkirkxd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glsgzjrtk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.tarul.cn/Article/details/geqjhrxlq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/gwzqfuibb.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gzuqgflur.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gocazvxjf.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gkkkqpfkd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gjxrofanh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gwpazmtxb.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gxsuvgwbh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.epnwcf.com/Article/details/gqynasulv.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gumaioopu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gkmytwqya.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gjgfsjdcp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gotdirczm.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gsauwmtjm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/goophzlzx.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/ganvzeavf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gtggnyqtk.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gsxqofucr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gaejzxjhp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gagwnzqaf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggvvhlcma.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gzhsudato.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/grbmbjprk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/gedvqaxkn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/glalrqmft.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gdsdtdclr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gbimientb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.epnwcf.com/Article/details/gacyhaytp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/giccsrrip.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gytwztzjv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gfqygwlzz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gncxszbnm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gcleofvqu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/gzpigkfqd.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/girwdmqon.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gnopjtyrz.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/ggvcrzcty.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gerwfcyby.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghbwkylnq.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gfvpektjj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmsxihhma.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gyohfawlu.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gisgsntrf.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gilcaxdrp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gctyolgsz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gkhavgmaw.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/golxzgdsp.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/gldbbkozp.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gmdydfswc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/ggqyzilfh.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gazalredo.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gvnbghpxr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gjyuhdcex.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/glzuuzvkb.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gmqqhduwz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gudkumffd.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gefmnhqgj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/glbzqprom.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gmntktgeb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/glyiwvusb.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gdryqorqx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gizkksazk.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gxzjomsnu.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/ggxfxtwco.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gbmgphyja.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/ghykbhkyi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gczokiowf.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gdudstxrk.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gpzjvurok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gzjvxgxrz.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gkkoujfbg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gukvpsdru.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gmojihccj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gicikcgmj.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gyowhmyub.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gnepwkqna.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gebfafyed.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/grxppqswh.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gojezsdzp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/guuuxwjbr.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gkbnkrlcn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.tarul.cn/Article/details/glinlasan.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gdhvowznb.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gmsjeihdw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gwgncxvwc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gljqcsbas.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gdihbiixp.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gfjtybxij.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/glxoxofvc.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gtwodpxnz.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gomgccymm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/ghbsgyncq.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gzaopzrxl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gbhnbvbjh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/geprtrzwu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/ghkvqqlsg.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gchhmrvpy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/guhtvasgu.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gupjtumyv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gpcqfotag.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/ginvayefn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gwjzjvxvk.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/ghrwomuxy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/glugqcexj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/ggqzdndcy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gjfjncvxh.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/ghnnsuodn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gochezymy.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gvlcoymfo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gdieihgsc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gkaykgoea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gkuoxryca.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gbbwwooio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gdjwbyxme.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gunejsxgf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/gpzjdnxts.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/giiiyzxoi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/grvzdgomf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gojfkkzme.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gvgaqsbsk.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gfknuddxy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gjithjgig.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gimgyfkly.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gwngeotpq.sHtML

[R40] 追加写日志
来源：http://m.share.fktsv.cn/Article/details/grspwegqy.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gmwqfbzaf.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gxfzmczvm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gwmzixztc.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gygfhsufm.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gbeekpgth.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gugfibyxg.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/glmoytbcn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/garwhtfnv.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/guffhrlnp.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gbervhnmu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/guohnqyig.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gqpexefyi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/ggpudimxr.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gffdwgntn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gunwpvdmq.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gkleofjsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gaetpontp.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gxfwybhmr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gxquwmnmh.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gzqhccerx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gdledixtr.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/geplkfmvv.sHtML


<!-- 参考信息 -->