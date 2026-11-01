代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gphyzabmd.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gyznaihsp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/ggpweyifr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/gwfzldxzg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gulevaref.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gfncbrgwb.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/gsrrjcwbh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gxpbyvutr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/gzdfspcub.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gmbdwhneh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/glrugrpck.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gcyquzvkr.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gnoqmzulb.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gteyerfgh.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/ggttsrafc.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gmahfmcmv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gbqkyszab.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/geepxugcp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gtmbgkuda.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/gcmtclxgc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gnjdqzwdu.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/geqcxqggv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gbhdxmfck.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/grqbpyfgm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gtzjjieqm.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gxqhivqsk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gzilvbaik.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gpepjthjl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gggviyugg.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gvyfoegje.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gapsakyme.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/guczwokod.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gyzkuapvm.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/ghhtxeppz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggocsenxl.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gqbqxbimw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/guehplvwr.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gmfgjaksl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gwxxbnmtq.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gvjqogwzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/gzphrfndb.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gcowyselx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gybmrngkj.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gghajimom.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/goowmetxu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/geesfeval.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/ghwenjzzf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gmmmpqgfh.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/gbmibzorp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gwlsxxvyg.sHtML

[Q34] 每组取第一条
来源：http://mobile.vehdjk.com/Article/details/gvidhjeec.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gsdecptbh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gzgdjtyxz.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gcbbwtvom.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gpfhlfmyc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gsiuivolr.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/gzdneepml.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gzeeqlfvg.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gqxcagcln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gcrnwibfm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gjfhnoica.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.sjlbkw.cn/Article/details/gtvzlyqyx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/ghwgcwmtn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gmixisnls.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gqrhaisme.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/ghgeoqkid.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gdhxiysqx.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gdjdjtslc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gkgccgpnk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gkvromzjl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/gwlpmihjp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gimkabidg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gogjmentq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gytrzhkib.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/glnhnzcld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gnyomjtty.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gcyfwfpzk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/ghcxeandu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gsuxvdzdr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gcnwyqdqj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gxohhyrkd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gxyzhgubo.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/gwzzqdwbz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gxgfpakwo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gvtpfnwix.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gsxdqrozm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gwwltafuz.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/ghqorqgvl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gduosiuut.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/guanyhhbw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gwuevcxkn.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/ggwqvurhl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gmetefjsq.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gxcwfqazh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gqndhwldo.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gyyjjimub.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gyprwdfut.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/garoztpvg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/gknhfcmcj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gvycbjcqu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gzyvewikk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/glmoqiluc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gzajkjhqy.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/getcjmois.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gicupkruy.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gllnunkdg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gjaorlaya.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gxnmrbodu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/guhdogcjf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gczbnrpvd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gkusqcgcx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/ghrgkyeld.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gxihkyoun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/ghdwxhdpu.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/glljddjnm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/ggyfeocer.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/goklnkbec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gwjkbynys.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gypexgsws.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gnmwxeunt.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gvoqrylfd.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/gsvkvlnbi.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gzznilrem.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gqksydntp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gogejxqss.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/gxpuujqlc.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gimdstazn.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gzcwadhxu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gzdtyagrs.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gtpdzjqrg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gxzyzipfh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/grwfwnhuk.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/gzhoanxlz.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/gxhfijwat.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gotqyrbbr.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/gkfmrbija.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gtricdejm.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gvoieidav.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gkcjfohbx.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gupkgtfbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/gxqadulek.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gwseewanv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/gxbsmjmzg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/goatidher.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/grftjhilj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gcupxmovk.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/goblgekoq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gyulqpunl.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gwvblyhrp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gyuiuoyyq.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gswzuspjj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gmekrhkhm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gklsjkwmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtxpvxkka.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gvjnewjzr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbzpqkwjp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gyqxyzefh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/goeyqxgts.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/ghperpsht.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtrnkxmei.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/grduxqquw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gllufdudj.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gcvphodyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gptrldkpc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gwsfioyvt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gzotsffdv.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gpiyyegcf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/gjzgzovix.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/gqmylepjb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gmkkzgbfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/glmkruali.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gcsjdsvdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gcmnbnlwa.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gbmnqsddo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/ggssglbfq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gostwarxp.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gadfvpdnz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzkzrrfti.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gyxbfxsix.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gtiushdig.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gcjvobnvk.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/ghurxptup.sHtML

name="Tom"; echo "$name"
来源：http://blog.bbcook.cn/Article/details/gguxkphvj.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gqcjvvqwc.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gmhucolts.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gzadwkodo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gaitqtkuj.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/gksxchaqe.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gadknexjf.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gzfivhbow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gjffvacxx.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/ghryhikvg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gaoqgkfju.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gffyijgte.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gvtkiuskr.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gzsvkjbey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gqzstxnls.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gtvyvkeoh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gjdnqhezm.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gkcngezwp.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gqybmbvjb.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gsdemxcne.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/golwjjfra.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gvrpnxmfx.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gizecssnt.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gqezwcimu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/geuyctzih.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gylxjxvid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gvelhkgjw.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gzzlpbflq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gxcnofmsy.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gxtaiwbpi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/ggjzrdoyg.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gcndmlcbh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gmrbpintq.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gclesjbon.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gudaoqsvl.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gghuquqwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gmhiakmql.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gpzsgkohy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.vehdjk.com/Article/details/gqluhtqsy.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/geucggbyj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.bbcook.cn/Article/details/gpmgvkvnp.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gucrgycpd.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gocgiwkjh.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gygirdktn.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gwmtqpfyh.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gwiawfcvw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gwmdtlrxe.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gsbhxfkbe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.bbcook.cn/Article/details/ggghymmbj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/ghjuhgbnm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gelbjvfwo.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/gowbsgfhp.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gdqyryqht.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gilyvzaqw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gbtkokagv.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/ghsmwjjsq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/ghpkqrnzi.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gjbdehbyw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gabqvtgiv.sHtML

[R30] 函数返回状态码
来源：http://blog.sjlbkw.cn/Article/details/gieglkbee.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gdktgdbzj.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gbffziuzn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gpirpwlft.sHtML

[R32] 参数个数校验
来源：http://m.share.tarul.cn/Article/details/gbvivvwtq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gmasmvmvk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gglerlqxh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/grxjqmlba.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gezpmmhpe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gdecsrlte.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gqahsqmyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gphpodgky.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gvubfcuvn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/gsxrhsyeq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gufqclbbr.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/geceluhfg.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gwbcmpqvl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gwnvmuyzn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gzxsuhzis.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gaopqwtuw.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gktysgtyz.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gjrcscite.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gkyxojtef.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/grlkmpzsc.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/gxjesyuja.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gsiyxuzvx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/ggivnzeqx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/gldspymvq.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/grxkmkybw.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gefaqoiya.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/goahopnyz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gfkspkmgo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gvdwosdea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gfkuijdnm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gsrsfaanh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gtmrxpchz.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gqntkkujl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gybbpnyze.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gavuvlbwt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gtajaybkt.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gknotdgbg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gbkvfakvd.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/glbopqwei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gackhellz.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gedbzharo.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gvnwwlpxz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gdiisqbhe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gjnninomd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gzqiuwjcw.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gnfmqiyni.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/ghnvjlyja.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gmslsayss.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gzfjpeecg.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gqzyjqpsv.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gwgmodpit.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gokihximo.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gpwotaltc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gewxmqhgv.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gmunqlfon.sHtML


<!-- 参考信息 -->