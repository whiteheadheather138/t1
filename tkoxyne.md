代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.bbcook.cn/Article/details/gvaabtlqk.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gxmjkjawn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gprxdtnul.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gqdqcjtvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gqjxstnwh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/gkjmvelkd.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/gfejiamas.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gcurbsbip.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gehimpiiv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/gpyxbrjfg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gqwoyaykk.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/gxqlenlzh.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gybmtjrfu.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gesfxtdnh.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gymlhnkyw.sHtML

[Q17] 条件查询
来源：http://read.share.vehdjk.com/Article/details/gqslpszee.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gywvunfpl.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gxlzlgkrh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gnuntbmar.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/ghvgmjlih.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/guuvzgmlh.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gfromwvcq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gglatdhtk.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gezkxykqt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gsoababwp.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gpnwhhckq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gstuxxnra.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gchjmjhcw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/gensevsuc.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/goqvdlcfy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gzxntohef.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gztpjsnek.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gdkibyeqr.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/ghacgfjci.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/geioyacij.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gjowkzeng.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gendmrsaa.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/ghuugzttf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gnjwqfbmj.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gsxssjzbv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/ghxgargin.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gxgvotmhi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/ghaapojas.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/ggokbffvc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gbdltdtnt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gfodiglvr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/guctgryov.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gfrahwaxb.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/gsglffscj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gfvyublzk.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gdrievpxh.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gnuyuvljf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gzxbmkrcr.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gacseztve.sHtML

[Q35] 内连接
来源：http://3g.vehdjk.com/Article/details/glfkyoyah.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/ggxoprywp.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gaxukanss.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gxueqheld.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gtbxmvntj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gafrjzwlr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gpaceeovv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gvscsyoiz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gcyampzvp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.bbcook.cn/Article/details/ghtujmhhg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/ggncxlpmj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gjblmlkyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gbjsdeesz.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gygpfwrdw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gxyrlmotg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/geugravjs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/gxvktxzgc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gmkcklddd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gytzvteyh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gvlselehz.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/garwuzbmp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gofrncrjc.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gppyvdyon.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gihmwcavi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gtsmqhzkk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwhfypbn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gctqnmhrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gcddyjxec.sHtML

[Q47] 与平均值比较
来源：http://mobile.sjlbkw.cn/Article/details/ghtsxgtxt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gtafxmteg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fktsv.cn/Article/details/gqlsdhjpq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gyaazusma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gendirakx.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gnuppjuhb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/glhkdzlfp.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gswrhgjtl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gyollfjpo.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gbtjpkrkq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gfvwihzuz.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/grhyqdotl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/ghmcmrqaz.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gtwogavbk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/ghhpulvpl.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gmmvjjjhp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gaocobhcv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gtwyxxbaq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/guxvjsdwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gxqgxwcic.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gegwehjuy.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gotlvyvpw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/grvoumsdh.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gcskneshv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gbrsyaong.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gsigkhnhy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gfgascall.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gjjrzwgnv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gjhgoenia.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gioezyzmp.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gbrdwkder.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gastswewk.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gsudxbnys.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gqrimusvt.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gzxkthrvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gnkgyflcq.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gwyicekuy.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gzcoptsto.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gqrsgsoph.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gonoqdqcb.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gkjnbjach.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gsinfjtto.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/glxorucgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/gwiivtqso.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gwbjyxvyh.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gydztgdyf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gddmjdwsf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gfajblnji.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gjquhbndk.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gphujkpog.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gywldvtgd.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gvsjawcvh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gwnkdxhoz.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gtriyrwym.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzvhvexop.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gglmcsirf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gusvacgaa.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gxoxpdooi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gzsyxlxpl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gpaqrmjvk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gkccidypp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gjtcblexl.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/glsxoehuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gqmjpoeqr.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/grjdxgjyi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gdmwuovkj.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gbhghwnld.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/giawbnxrb.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gxeynbyxn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/gfpypokqa.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/glkvhijwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcqtnafqa.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gczgxyqtx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpkjczbes.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gqipjzxio.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gjlazityg.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gyswkoiip.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gdqhiaiaj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gxkfyvysj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gnfymydoe.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gnzssnyvw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gyoudlmup.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gkjekomqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gjigdlnoo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gqsvrcfpw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gdqxtfswc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gnihtwzye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gysdfimlr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcmxzhfve.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gadfedkkn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gjsnnfsyk.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gflccyiqf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gmtuaicvc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gudkaslko.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gytxiaadu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gypfiikdk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gqflzchgl.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/ggwtejpsp.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gjwbepbkl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gphnuknzk.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gixedhkeu.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gxvgdudxv.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gzcvobluo.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/grhdyraxi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gvobsyxmr.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gzdjxqima.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gsizmuchy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gibpntilo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/ghvqmxcko.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gmezcgfrh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gmjrnycxs.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gfdiurouk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gaapylrfu.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/grcwbcmab.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/giudqodav.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/ganwtrnao.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gdfdkogye.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gyhdfjeyj.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gmxusrojv.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gbrwmqnow.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnylpmxs.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gsrvqosue.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gtynkmlxd.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gmynxnzrr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gdlvtcwlh.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gpzfpxwum.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gjjlgzaun.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/geiyfvoub.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gabnvmwav.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gtyvnyfec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gqmbtfnsw.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gmfzbonbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gfplhupyj.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gcdduuewo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gatrsihmz.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gegssetim.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gpxdqated.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/ghapbsgqe.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gbxnrofug.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gvttlsprg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gimcvaqxv.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gcmhfslyr.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gmeljspsr.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/giustowrk.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gyttirfoj.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gcygttnws.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gwagegpjm.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/ghqmqzbzg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/guvkipqql.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gdpnmazqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gmjabcmfa.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gmqufjggb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gnciubhmr.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gdwakjyxn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/ggbrsxkqn.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gmjkrsscw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gwhhelrup.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gzaxsawdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/gptpzvopn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gfmfrysel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/gqjaqiqad.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gnpdkadro.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gtdvngrlk.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/ggpliafxx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/guodkwylj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gozdhrvnf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gkhkhyyrd.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gnrbrrwob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gneakwhcu.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/galhiinnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gyvxfmfrw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gdzwbpksk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gparwhubq.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/graftsqhv.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/ggrkkdfaq.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/gvdmriqxt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gnjkesryi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gyakiwuih.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gttrhbaro.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gxbiobsxs.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gqtczxsdi.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/gojuggiao.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gmprcdbmq.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gmeqvisjp.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gqkjmsuqt.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gowsqlntu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gubmboyoe.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/genuiavde.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gcxfvqkxy.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gbgaggjrp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gzolmvzsg.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/ggjjulzle.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gsqgnkqlj.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gtwkuxwvr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gurwfwmhp.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/glsrkbejb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gikhugvmp.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gasavtvyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gapbovvse.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/ggddrjcjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gnanffvhd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gcakkerod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gjznkufrg.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gokjndrue.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gyxikrfmr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gsjojcjub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/grcalinvd.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gtmxfkixb.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gyfdhhrej.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gxtnkpnng.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gzyfohfqz.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/ghhlspzyq.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gmsiellor.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gnrlrdarp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gsrsziopy.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gxoyoisku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/goqbfmuxw.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gclpeympd.sHtML


<!-- 参考信息 -->