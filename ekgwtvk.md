代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gpqsgmolp.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gsshdiujv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gwriwemev.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gaewhxugn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gegtniuny.sHtML

[Q09] 创建唯一索引
来源：http://wap.bbcook.cn/Article/details/gjuclpgzv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gloduuomg.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gnwbrpfmy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gmedandpi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/guuzbolpf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gknsabsvs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gdictyayp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gocnbbqsq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gmmgtfpgs.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/grafuront.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gbnzlhnnw.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gefylkswd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gqthrexoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/gckixakar.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gnbcnzsqp.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/glfiywyzf.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gahseupza.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gsokjprvj.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gnkahaklh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gljjgfgwc.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gercsowys.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/giawuggnq.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gpqlxoigv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gakvjctgv.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/glgfwwoip.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gycmohjon.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/grspcfbfj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/glmfmgxkq.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gwglremob.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gaqlmttsl.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gihkaelvv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/goybmgqca.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gpsyiaixk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gsqqszbhv.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gmgtbxndz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/gakfqjuyg.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gdnekjzkk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gqvgbwumf.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gimqbubfk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmdsfajhz.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gniyehojr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gflthkfaf.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gewdumjfw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gskivhicz.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gpdrdslwq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gybkmmflu.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gdtcsjjuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gpbwiemga.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gyrfvvlrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gbjvbpivq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gvbgemztd.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gburdbqoh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gihiryoee.sHtML

[Q34] 每组取第一条
来源：http://blog.fktsv.cn/Article/details/gdzkziqmr.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/gttxlwusv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gvqjohkvf.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/grenplbri.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gxwfbxfxp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gsaajsuof.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gxyuaqfew.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/grgymfebg.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gzpweqsnb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gqlesicln.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gmgvnluli.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gcxsptkou.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gsweqjgxm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gfsukbddf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/glrsmjdvs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gzwzmnboi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gzsidjdmg.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gqlphsbbx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gunnwrblv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/gqoldjrks.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/grvdtzget.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/grnzbnzcc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gztsuejgh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gffsvvwiz.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gofflamfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gxxbhgyya.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gexnxnlhs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gpodfzcao.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/gtotumluu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gpdwzpjce.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.bbcook.cn/Article/details/gtcuvudbi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gqwptntid.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gfqzgeojx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/glsevbzzz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/gybyezufm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gcuchlcqk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gftqrgaxq.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gvfndhgan.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/ghwzjbhxf.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gxmdxxuer.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gzshnuutj.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gpphbpkjd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gfemtlxkc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gejfoagwk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gpibugjrz.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gymywxbvk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gbkxbjqdo.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gdxeesiry.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gsipfdepd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gmgttcnnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gcadpfyei.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gtbyvpnpz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gqgkpzqat.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/grzqwwess.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmaoebkaj.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gjaewxxof.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gakggcphn.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/ggdgucmza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/geyncovdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gbklccone.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gbjsimuym.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/geoqhhzdg.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gebxamxja.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gehjnqnkm.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/ghfltpstq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gzxguycdb.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gqbzxmpyh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gemydleyi.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gvidstlff.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gsdaxkicc.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/ggfoxxudm.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gzpihkkaz.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gibxzaozq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gmvogyrwh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.tarul.cn/Article/details/ghrwfqlqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gxbwaimap.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/geotjyypt.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gvuhzgjoj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gtmyibvzh.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gpibudyqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gjtnxvbbh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gkqwgeuxd.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/ggzlqhzqu.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/ggycwzbhd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gfaqqwncs.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/geyruvgge.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/ggefftdxv.sHtML

[Q73] 查看表状态
来源：http://www.blog.vehdjk.com/Article/details/gsarmcghd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gskptvpor.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gqyjpjuih.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gptuvzgzg.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/glbukllsk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gssyyvmmk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gjoojkcnb.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gibzifbcs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gotjatekp.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/giizufxkl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gdtwbyepz.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gawtncpjr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gjkxoimpy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gbhbxpxto.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gjqaklcbs.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gkzeqccao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/goqijelwt.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gkgvnrssi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gjtnssyvl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gciwxkecu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gjajbnjok.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gxzgtjeut.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvhsvbqur.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gxqqaycvr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/galgmntll.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gmcxrwdqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gsfammlky.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gypbaopcj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/gfnubchnv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gnnttvekc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.vehdjk.com/Article/details/gdobbozee.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/guhonsvls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gmjuyzlel.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gojdaggta.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gqabcdpsj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gukfnwxkt.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gxyspkoba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/gledtedpm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gumukwukq.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gxxkasshq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goclgcqic.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/glwhyckfu.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gdwoyojci.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gnkoohtgm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/geeyecsgh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gtufdtlkc.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gpqrzurka.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gtypbfzfb.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/goppqkyce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gprnwyvhl.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gyqgvbdbe.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gjopaieix.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/gvpwpmsmb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gxfxxjssf.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gceckoapz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/ggbvtwkra.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/gwdxzyevg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gsxhzfjrh.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/gpsucgqmh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gokkazdtl.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gotoqmdef.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gydpwuyfy.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gzgmlwenh.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gkxqdgsao.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/ghtjrursb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gwiynanar.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gileruwbu.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhvbsusn.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gxzyaaxze.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gmdxjimhx.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gbyfptsmp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gxpswwiha.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gtidhqvur.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gwcblplhr.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gtjuyoprl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gyytgpkxk.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gxlvzrwnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gfqndttjk.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/glixojkhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gwivlrrco.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gjexnbxav.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/gybrphntv.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gngxyddka.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/ggovoeuju.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gqmsjewcj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gsvmwhqbj.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gnigcnled.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gqgaqnzmc.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gehnjzdjn.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gwkfxbquo.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gewjflsdx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gsygtfwac.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gradahbqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gzdzjyzgo.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/ghggxqbyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/geabtldie.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gawiqtoog.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gywchbgpl.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gcjtfnuxw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gkjdiqcts.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gpdhkxwst.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gqaoxmsbz.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gagvokrbr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbtewdir.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gavehuhzw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/ginbugekk.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gpyvdhbqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gruylivtt.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gnpfdrwne.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/genykjrup.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.sjlbkw.cn/Article/details/gjnqzkiwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gdyysqbof.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gzqbiibrs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gpnxfyjjk.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/gzxkfhsfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gtxaakcwu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gonxizngp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/giasizawl.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gilklxgpp.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gonfkwmqn.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gzugtvbgf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/ghxyjctxm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gvpjywbim.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/ggtigecem.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gporwnvhs.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gpngcmnev.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gesyjfpyr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/glkscumir.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/glgltqeur.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gzpwgsoqs.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gmlopzqcl.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gtaucbqdg.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gwfarvecm.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gawuehoot.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/giucalgwf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/gccpjzwnl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gsxjikabs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/ggyrnzolw.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gyubvmvky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gpttztcja.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gaiqqdsaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/glzubiexo.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gcgenrcss.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gptqebbdn.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/glgsfibzd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gxzvlugbc.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gxlnozpcx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gbjqhrzxh.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gmjlayzqe.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gnuhxkfnt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gkzwmzzfi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gohdfypwk.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gdzsovgwu.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gcfbwjdwv.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gnyahzjaw.sHtML


<!-- 参考信息 -->