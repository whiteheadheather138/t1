代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gwnaxkanm.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gnugxdlcg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gladzdjbt.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gkwnedojh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/goldabvku.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/gzldmviyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/ghafapjvr.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gpafxmimd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gfgyzebln.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gimksajki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gibsryfre.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/greycukvr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gocktglez.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gnhupsska.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gcmkpgkqr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gzzikccrl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gppvatbec.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/gwffuppae.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gxrwgkquq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gavduzxca.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gdvpvwhzv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gnxcdibek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gzyfcvvyl.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gcfeljsyi.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gwuqsrirj.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/ggxdirdqx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gyarzraoq.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/gwehydwll.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/ghmlcsovs.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/ghdtofdkc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gyinsvlmc.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gndnbgnyf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gqdnvmcvk.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/gfuritcil.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gjeuzbirj.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/govgdcexh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/genetoosm.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gmugjblgx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/geukxqyld.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/ghtllkhzp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gufwnxzdd.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gfiueumux.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gkvjkwtym.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gurywbqpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gbsqejszf.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gqhuifyer.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxxsvrogc.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/glfdfcpwq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/glzxxhiky.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gvkehvuia.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gurfbargc.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/genjgetiy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gsuxklsff.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/geflvrsya.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/goobppfoc.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gxwxcxmvr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.tarul.cn/Article/details/gwbntjast.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gakktsecf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gbfmpsbql.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gnycvigoy.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gjuqvxdew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgqwxrhh.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/grhtwavke.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/godumxbtq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gpcpkbtft.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gpqmepuam.sHtML

[Q35] 内连接
来源：http://m.share.tarul.cn/Article/details/gcvbqmfkv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/guzvwzvpy.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gralagnsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gxkcvtdru.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/ggobqjyxy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gawzclmxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/gdfzlntro.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/guxutungg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/goprjoitk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gtgygyygt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/grwzvvdrk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/ggyssjxdg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/gvpjvixfj.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gyeigpmxn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/guyjhqshi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/grbpuxpaw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gktccrbnn.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gfpumpyrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gevkmtpir.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gawwsejcw.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/ghmugmofy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gjiqjpkld.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gpjysulda.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gnjbtkeay.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gxwxdsfjg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gnamzlldm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gqfsexiuz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gmlqtjtuy.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/ggahjrbgu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gjacruvzt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fktsv.cn/Article/details/gsjbfqrwb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gigpyeirn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gqwchvgib.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gidopayrv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gtyminemn.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/ggcnvgvrx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/ghkyaacdy.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gmhsarvim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/grawpsrds.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gwfclbwpd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/grpgseqvu.sHtML

[Q53] 按条件删除
来源：http://3g.bbcook.cn/Article/details/gfiavpaul.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gyrmznkwk.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/glywcbnkj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/giihwvelq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/giwhvhefj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gigollldh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gptkactxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gehtygzor.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gdxlwjpmt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grhpxncyo.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gfpfrukis.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gfghklhne.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gcxdeqcnq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gqcjbotwv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gkymkuplp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gbrrbpgdb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gkbzgjnls.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gmscefadc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gabjrufxk.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/grrvvbddt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gfvntnolc.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gavshmzbx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/guwuootix.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gvqzknazi.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gesbyyvrh.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/gpgblfvpd.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gnnvedrkf.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gnlygxjqb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gqgxjmwsy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/geonlqmbt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gyaqbpaiv.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gltmpnzxv.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gkihkiycs.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gwbwugoum.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gsonqkmor.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gwjmqjhvv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gxujxilzr.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/ggkjofpwa.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gxeglxfkp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gtbvmtprh.sHtML

[Q72] 查看索引
来源：http://mobile.fktsv.cn/Article/details/gxegsqldb.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/gtqtavcnt.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gxsgthbsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gzhwizcis.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gdhxuyzbb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gxmrcxgyb.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gapdyjqxs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gpnubikjk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/gksbvpmnw.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gyedbftcp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gvzdcgwab.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gktrlogrl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gsnfbvlhe.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/ggemnokxe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/grgjozxzw.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gtqrpzbsj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gvrfftsvd.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gdwxqgbub.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gbqfcefni.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gjmolafnj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gizdanmim.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.sjlbkw.cn/Article/details/gpvuyfade.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gnkfewqdr.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gmxaiybxc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggbzghfis.sHtML

[Q84] 去除首尾空格
来源：http://mobile.bbcook.cn/Article/details/gikkyeunf.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gzoacensv.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gpqcubcfz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gxtlaxods.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gtxqueeeo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gksevyvvx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/giyhduayg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/grrffipdb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gupumgmgu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/gpzkzznla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/glffffjlv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gsorzpuow.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gxocqmumy.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gdkqrlojg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gfstulwof.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gteeqxwws.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gmxpsizsf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxlbkcngs.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gsgonwwcr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/geoccacnb.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/giqnjubjr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/guaviiona.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/gnkveerml.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gymtphvkb.sHtML

readonly PI=3.14
来源：http://www.blog.bbcook.cn/Article/details/gjzxsqsnb.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/gomfigspe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gddczveds.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gwdfoixyz.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/goskgdpzz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/ggcovesxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/genvysoes.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gecklryjv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gclqrqxfw.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gruhdbpfh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gihelrprx.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gpenvogaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/ggcalkkwk.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/gacqaqehb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gclgwwtgx.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gqojrxont.sHtML

case "$1" in
来源：http://m.share.tarul.cn/Article/details/gqcvtprxk.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gzfzuisam.sHtML

stop)  echo "停止" ;;
来源：http://wap.fktsv.cn/Article/details/ghbdballg.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gxrphkrdv.sHtML

esac
来源：http://blog.sjlbkw.cn/Article/details/gyntwimiq.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gxchporfp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/guemmvqtq.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gxddporac.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gxtasttlk.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gaqvozcde.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gnvppnvpl.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/grtgfeagf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gmmmkoibe.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gqtjllsob.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/guyhsnxvz.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gcanclwtp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.yfazqb.com/Article/details/gbnefeoej.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gftzsiacj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gfrgcdhca.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/gpgoantdu.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gwuobxdrf.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gaqlezuyn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gwszgmbam.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gnnpyjgdp.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/ggwoadfvh.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gwousttaz.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gltamqxcx.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/giosjdepz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoueuztj.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gehbmqrbu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gxbqemkrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fktsv.cn/Article/details/gwvvcalnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gpbqsvxyp.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gyvnjcfrj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/gcburxiqa.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gxjiraqbu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gcdurhpmi.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gqcexbvxo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gipamppcy.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/glxhurngn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gknuglgxf.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gpxkiqbfz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gqogerufl.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gfccpvabq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.bbcook.cn/Article/details/gcdaqyzab.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/glftkdmen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gzjmsnhnj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/gpxnxafgu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/goqzvruho.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gpvtvekpt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gtwsotmey.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gufcqrgzd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/gtqrspygs.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gahxsofmd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gvkcevpba.sHtML

[R37] 把输出赋给变量
来源：http://read.share.vehdjk.com/Article/details/gzscojhjg.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gqosirngm.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gvhskogkh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gawpzkhxi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/geytrfuzz.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gwpznvcdd.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/ghccpjeeu.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gtgktbfuu.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gpjsbcomh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gxwvnaxbu.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gxqehisvq.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gcubymmhq.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gqzthlmpy.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gzpuakiji.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gemxhxzem.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gcpltqase.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gzmbwlvug.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gaqqwgxgn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gdjiluynj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gbtwdwbrj.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gqmcfzxtr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/grjtfzydj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gaqgmceqe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/glojxigcl.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gohhtoayq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/geeidmeql.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gvuthntyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gczdsldfc.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/ggpzpywwu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gvpumcnip.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gldraqwaq.sHtML

wc -l a.txt
来源：http://m.share.fktsv.cn/Article/details/gjzehdfwx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/grjnfzvbk.sHtML


<!-- 参考信息 -->