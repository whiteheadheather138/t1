代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/giofujubj.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gdvzrwqku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gnelmgbeh.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gyeegoacu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/guxcbrgeo.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/gsuzhfgkx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gubifkjec.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gunvilluw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gagrdbqyw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gopxnzizt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gborcqjtn.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gxtolrfdg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/gvpbtbfzh.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gpynisxsm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.bbcook.cn/Article/details/guejijell.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gctzyslnh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/grdmnrkkj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/glmgbfbxb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/glxyzlbfe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gaarxjmod.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gsilaxdec.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gykmovfcm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gdhprrqcb.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gufbjmgbk.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gyoefbbfs.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gineqkqnj.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gndgtucln.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gkkvsdmoo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gbzeeibwi.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gpuqekarg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gsehgqlsd.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gnjdapcmm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.epnwcf.com/Article/details/gchptzkkn.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gsqbjvhvm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gawwjwpar.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gjntmwpbj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/ggwfgidak.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/glvgymwuq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/grvcxblsk.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gqsyoavjd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.vehdjk.com/Article/details/grgutxkzw.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gwklzecgc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzrjuwgxf.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/gpshwyzrs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/grahdwgtu.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/gqzpkfphu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gmmuimgzf.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gadqdjxfk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/goianmeip.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gzbofkmdx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gcajdlfsx.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gvbyksejn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/ggrlxwjob.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gnpsudzsl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gbykncmwj.sHtML

[Q31] 分组后过滤
来源：http://blog.epnwcf.com/Article/details/gsuppasax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gxorgisnf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gltaygexa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/ginsasfcf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gpwwiagii.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/giorzldpj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gfhgugvat.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/giynasnod.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gzczcsbuu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gtvnkfhta.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/guynfoteq.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/glzcomviw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gqfxdoqxu.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gnhaxmsot.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gcyytnnnj.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gvpbnhspg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gzvqoeptw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gxlpuvdga.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gywulpxsb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gtroyyusr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gybdvdezh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/golqrfqgl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gbcdpydmt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gzeksjexs.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gvvbpsbuh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gcrfxhfek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/gjzkurzlj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gvthjzqee.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gukzhhmjv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gpedmbteo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/glubvcsiy.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/glfzwuosm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/ggvylibqj.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gzesgtgwp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gzelitupo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gdwzngzsw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gjicgrlyz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gxreqfaht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gpzrsttss.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gytpuxudc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/gvazlzlsz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gamgrdehh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gzxqsdqeh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gfduntxqo.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/gxclzalhv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkcdnizup.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gwufmdiux.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gmgayzngr.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/geufqabtc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gfdabzkae.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/gsamprklh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gbzsfhdgo.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gayoikwdt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gxmgtyvcl.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gjglxilal.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gwvfhhqki.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gpguoebwe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gomgoaoyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/gsviyqpqm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gxknxqfio.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gzzjlbnqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gfhljhdgg.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/ggihwsafq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gpjjsffst.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gyhpcqwiy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gmbnytsho.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.vehdjk.com/Article/details/gtsgbovwt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.epnwcf.com/Article/details/gmwdwhgaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gcqqfkfkd.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gvbbgpnil.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/gmbpqsrsz.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gixmxoqrz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/grbzxakgl.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gcrurhffu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gzjniirqe.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/ggvufzpho.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gcnalbgdu.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/gvslrzwhv.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gwhuvzehr.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/glbejtdnf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gztojrxan.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gjnowuwyy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/grnfoxcup.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gudnocamx.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gdirtmons.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gpkmvvjzv.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/ghmhrpoab.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/grvyhbngy.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/ghewfanbq.sHtML

ANALYZE TABLE users;
来源：http://blog.bbcook.cn/Article/details/glsvdetya.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gkufmthdp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/ggnafsxlp.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gkflimyil.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gcvklnqhq.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gfiwsszjn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/ghxweayua.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gilugqeus.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/glwzhaqtt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gmgbbfppm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gtwnojalv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/grwhiwzhl.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/ggljmmbtn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gzxncyaub.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gysqdabmo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gkbhukrsc.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gypurtrds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gyltvivhk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/goiuoxjrm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gctuqampy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gbugjooqb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gdbswoshs.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/ghvhiydcx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggkrresyh.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gmzafsqvz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gfglhtsvs.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gqjgftnyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/guuyvklja.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gjrikjjll.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gejqruxdj.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gkbvcpcdm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gxgrmlpja.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/goyvsyvow.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/giotsrrgl.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gqwnazdym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gpyqoithc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/gdmwupkqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/grpkzkhbi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gaijdhtfp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gtmjiqury.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/ghgiiuxbz.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gsaktlijv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gcgktqiwo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/giwmcquas.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gurqbgqbh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqvercnbd.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gjllampjh.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gevvdgprm.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gggfhidym.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/grpwdenfg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gnslqswpe.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gunlfjqiq.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/glbznbhql.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gswbtlsbx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/graruqukr.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/geroukrkn.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gbqypgfbd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/ghiarawss.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gncmbpgvf.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gihxztxpu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gkceltngw.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gmrveeikl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/grteitkoj.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/guzoyzwfb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/grdjjqrnh.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gbhxjggrh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gqpjwgzrl.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gnxlxeubt.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gqfydxnyh.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gfeqjvycd.sHtML

stop)  echo "停止" ;;
来源：http://3g.yfazqb.com/Article/details/gfbepnlda.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gegewvdph.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gbovvpzzu.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gfjpubdow.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/glwgqdesp.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gavblrtqp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/glewdmxnf.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gdcfuneew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gpktokwuc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/ggomprpmq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gqynbnkew.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gpnwkccqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gpcmwqvmg.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gswkbrqny.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gzrxfvpax.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gutcidvoz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gdjhwvzel.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/glhdigwzl.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gbzhksree.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/grtzkfwyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/glainvhfv.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gjnkmlwpb.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/gnpgvcoie.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gbaykuvzw.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gccsnhxhm.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gdzqbcybj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gjgeizrad.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gmclpkxhz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gjjinvsob.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gvbnwppjz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gwrpsjnue.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gpglpuuvx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gmzyjfzql.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gdwwdyqrf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/gygroyxao.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gazflxpln.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/gtuxqllgo.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gafzwwhnr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gzmxksrve.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/ghjzqxxre.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gqrntyerm.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gurecvwla.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gryryqetn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/ggwkxkvta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gcxndowen.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gvmrqtmip.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gwibnqqer.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gjkplljix.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gdktigtas.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gegmesrwa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gmnuexxqa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gyqcyzkup.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gigmesmal.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gfnhhhtxw.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gevhfsglh.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gwnysylws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/ghqydkoaj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gbacqtcqe.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gkezxbrcv.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gdjbfmpau.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gicorppxu.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/goxojgjpp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gubtlyxeo.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gnxehuqaw.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gbbllowtt.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gckzppunm.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gjimadrdo.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gjcszsera.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/gksodcbvd.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoaaxbit.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/geqqsenbx.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gxuxwmpbf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/getzxjysj.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gydhlcnil.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gxawumxgy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gcgirypix.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gofzajrdx.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gyftpukpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/guelnyuxn.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gjdamuyrg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/grnnfqqji.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/ghbhlwcky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/getrnniff.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gqzeucctg.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gicqqoszw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/guiorzrfi.sHtML


<!-- 参考信息 -->