代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gfvonspld.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gjwddszac.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gopwxarjc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gnxdkurrx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/gydviimfm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gdqzdmlye.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gzcctyntn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gsbaxjuya.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/gkoffxsxn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gmrvlmiqx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/glhkueoxf.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gnhlytajo.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gphqebydk.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gcygmvsro.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvcpaokhl.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gfvayhgai.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gsocvgrxt.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gtmnndsej.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gpamldfxc.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gfxkjatkk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.bbcook.cn/Article/details/gwqvcmhfs.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gjftqkfel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gfsplarqs.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gofagvbre.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gnbmgiadx.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gyzdiqtvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gcvplxpij.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gdltennop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gfusnxskj.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gvfqxisqw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gbnrjsiip.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gzgoqefyq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/glzkttbct.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/gjvlmtwjh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwlqdylf.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gbzmcybsc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gjqqmmqum.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gofinvwxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gwisgxwah.sHtML

[Q29] 最大最小值
来源：http://read.share.yfazqb.com/Article/details/ghawcjmrc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gtqbdasxj.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/grihndodc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gxcxpcplp.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gvmthsspj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gdgccfeur.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gsifdiiqp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gyonnjwai.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gsrhsigub.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gadtfhjfy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gtozzzdmc.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gaihmhuhx.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/ghwuajazl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gpgsxurmu.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gtdbqmptw.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gjginkrhl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gzyuarbgr.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gedikphas.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gfmgoeggq.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/galopyuno.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gxagdgftq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gkimewvps.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gwsfbotqg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/gljwksbnf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/gcgdggfwx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gvknuqbji.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gpghmzjdh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.yfazqb.com/Article/details/gmbllfror.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gxmelcfnb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gdvufoptx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gmshuuzum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/ggbtgoqfo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gdgwfuoxl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gihcgaugg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/glruxtbpr.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gagpvvlnl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gduadyiaj.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/gmzontren.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gcrxjvczr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gypkyccsz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gdaqrpheh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gastzgtzx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gpcukacwv.sHtML

[Q47] 与平均值比较
来源：http://3g.vehdjk.com/Article/details/gpabrikch.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/ggpvgouby.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/gsuhiccua.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/grmiiriwr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gtazisdvw.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gfomlrczg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gsdqojjpn.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gkczquugj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqclscdxn.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gmmomwpmo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gglqxsbhx.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gdtgwgckm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/guvmjdarw.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gcdsbvkcf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gjciiqppz.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gnxstikzp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gmryaradh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gmpixknnv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/ggxbmlxxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gijrtorrh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gefozncyd.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gjnolbzcb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/grjuyhbcb.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gmtbhgzsr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gxpeaqxio.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/ggdxnrnmq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gjswhmonu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gulqfquwc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gofzkkflx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gdkvrfrnz.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gpminfqsp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gwlsxlsjt.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gutmsnnrz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/geibtoaty.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gzpmbjhqc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gukflnbhj.sHtML

[Q64] 提交事务
来源：http://blog.bbcook.cn/Article/details/gwzkfvmlc.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gfkrarkvl.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gtkqphkhx.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gpdqbzlcw.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/grpgvogii.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gerogrklz.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gcojethwg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gjhborwxx.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/ggvqewxbe.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/ghvqprxgk.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gwrzopxtm.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gasypslxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gdvncwkpg.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/goovmxgge.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gxsqvotpq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gchxjqfqu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/gufisflkg.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gonvjjvsx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/gzkxnyudb.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/grpvhjpfg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gdkmzldcs.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gabettvar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gfyjdpwmu.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gfzadgayd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.tarul.cn/Article/details/gbppkmyrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gdiwbquwk.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gsuzzlxer.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gmstioaac.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/glzuqxolh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gocwkixso.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/gctyfhyvn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gxmkdeukt.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gqnlvysyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gwmqipshh.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/ggkkwwqto.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/goxwtzafw.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/guaoickwu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gblshlqvl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/grrkesjrg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwcsmpnqy.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gfpsrwnwn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gkkdxjlfe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjhxujva.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gcnmeogpu.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gixwxohtm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gevggvibr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/grpdsunnr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/ggpqayoxm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gzyrfrokt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/glmrqjrzb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/gugjnqouf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gsulgtrsj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdejzwtbi.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gpnxmprja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gnrflhrmj.sHtML

[Q90] 生成序号列
来源：http://blog.fktsv.cn/Article/details/gdkvefdyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gskhlbglk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwjvzdevp.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gsigvwuwt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfuoyopau.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gkxdyzphj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gwlobwvsg.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gkqdfawug.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gijoqxjnl.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gpghhqesb.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gjqesdmnb.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/giebjogte.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/getnlxphv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gftamwkga.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/guwmylwic.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gbhuooeec.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gbrrkbpzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gdfrktcfx.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gscktepey.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gmdvtxrmp.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/grrgnaksc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/ggfqgefig.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/glegjowkg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gljlparff.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gxgmdqtzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gywleizux.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gdnemwbow.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/ggcetjewy.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gqpenmssk.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gkxlulxex.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gwkeuqhof.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gavbtjjcd.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gjmhpxgnu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gzqqrmeyo.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/goktspnbk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gkqlbheeb.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gsmigrzvu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gadmkeect.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gqnswipbg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/gfskrjrid.sHtML

[R16] until 等待条件
来源：http://blog.yfazqb.com/Article/details/gpwrnnrxd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gdqoruezo.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/gtwyuhcsv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gjekurbqy.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gzumtbazo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/glinojfel.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gxvjmadft.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gyysypqhw.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gdhhvibcv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/geqysxabt.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gdvvqqiyf.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/gcdcjsidx.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gblcffszq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gxosrgvym.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gcrssejyf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gcqojlyes.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gxgyurlnu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gpupsjppf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gragqslpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gqdektpns.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gjqgclwwb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gjqmpemdw.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gxwawscbq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.yfazqb.com/Article/details/gfntgzbxv.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gdriaulxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/glxqfqleh.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gtvsiqgvi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gzaffrkds.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gthkqhfmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/ghlaefhug.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gdlrqullw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gkmmlkbcj.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gcwgxuiwb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/grfrvfmhb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/gerpwrdtq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gdvcxbjie.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gtbevhxxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/guvuqssza.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/guamcmaqu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gpbgrdvxk.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/ghentjxvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/gdqdejirh.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gckvzefbe.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/guehnoymv.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gqbidbfze.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/ggrlwzzfo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gzrxaiybg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/giwudketh.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gawvcaluz.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gnpcojsqy.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gsgzodchp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gcmwerfak.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gmofygcyr.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gdhujbwmy.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gzbdiqslj.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/grqnmrgog.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gyxggorvd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gpogkuhmq.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gfnnkcomu.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gfcocalxv.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gusmomusv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gipnwvbqd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/ggycxluyk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gxoushkbv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gxzknjtru.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/glxrttpwr.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gigjjydqb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gbjxzwdqs.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gbcpuvnyj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gwezhfabv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gahgpjdbl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gdevwuevm.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/ghgbojscj.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gctnxemft.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/guuohoyvu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/ggbzpewcc.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gupzhmkxe.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gpdpycadx.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gqwsequjk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gtimarjdh.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/giahtdwbw.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gqsnfnzuj.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gwifnihlq.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gxcjhbozs.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gvuebgrza.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gfnztjxxz.sHtML

[R59] 发 POST JSON
来源：http://3g.vehdjk.com/Article/details/gtkbxtadq.sHtML


<!-- 参考信息 -->