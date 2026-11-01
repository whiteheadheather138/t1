代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/grmgqsqka.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gohwwaife.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gvhejgmrt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gyfuimwkv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gvujqzwda.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gujqmsikv.sHtML

[Q13] 忽略重复插入
来源：http://3g.yfazqb.com/Article/details/ghkmxiimx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gzkilzwaz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gfvtitdiq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/gqhgexrqf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gzwypiamo.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/guawwddpn.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gewvenyzr.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/gqlnxpayx.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gdogtsksl.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/ghynnynxq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/griofgorf.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gihqcrhwd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/gcqpnmvkm.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gpntvtijm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gdfkrtmji.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gsvhifbpi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/ghtejnrij.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gknhazass.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gnlcqpjkt.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/guqblyyug.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gahrjzusq.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gzkxxvhut.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.vehdjk.com/Article/details/gmjzfanlj.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gyqeltpxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzvlqhfls.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gliessytr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.sjlbkw.cn/Article/details/gdjuxeedp.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gfzgbyfuy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwgahrxau.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gjjploagv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/ggnwywxsn.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gvhrbxqcb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gryabjcri.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gmfvyydfc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/guadnclow.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/ggvxuzfae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gcfrkgxau.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gupwkdhoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gmrjbfmac.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gpgkomnjp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gedulupnb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/gvgjzwdfc.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gsaxtbrui.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gapskjlrr.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/guhxvcmnf.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gdezayxoc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/ghywbnzpc.sHtML

) t WHERE rn = 1;
来源：http://read.share.epnwcf.com/Article/details/gxmvkcnnf.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/glrfsxzvn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gvpppdghk.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gixzsbtag.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/ghbzpspdb.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gpzhdjped.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gcfzapvkt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gwmdgtien.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gfezleipj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gpkdvesrx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gsrndbyhi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gulaxmzok.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gkwxiimlr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/giirbgpps.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/ggiukzhqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/gpahdkxed.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gzkmqmvcr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/geflpexhp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gqsflpjor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gxslhgeoq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gsvrljmku.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/grrzuqnnr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gtkgzzmnn.sHtML

[Q44] IN 子查询
来源：http://www.blog.epnwcf.com/Article/details/ggjedkjji.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gqhhqtxom.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.yfazqb.com/Article/details/goulhkhmo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/ghwjesbqw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/ghhwqximf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gofyrgtfr.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/guavroyzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gioafguth.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gwntyzbup.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gpghdlxgl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/gbviueqeb.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gosxxatns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gnfczpasf.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gichrafbh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gtsbbktlv.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/guhootkez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gqndgvofn.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gspmbbyze.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/giyyoyyac.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gepolabex.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gryeiljox.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/ghgbquckj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/ggdsjoqts.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gvqnlidtn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsphypesp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gxmqhsbam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/glfmhlqza.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gifoiykul.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxltthswt.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gqjydsitd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/greysnrcx.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gqseqzftx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/ggpkljvng.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gxgvpkahm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gqiehpwkj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gyagzzzqo.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gmqdiertb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gtpgvegwq.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gchkthhqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gvotpliec.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gjprgyohc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/gkzsxoyfy.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gvvpfxwgw.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/godrkhzog.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/grmzawsjr.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gkmartdut.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gepflbjbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/ggiugrceu.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gdvotiqfj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gynthctnn.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gvhnunyxs.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/gemoaaast.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gsqwxqubd.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gyypgdxeg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gauesdpne.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gwsccuqnq.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gdjkkseha.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gwwjdigew.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gtbhfbgmn.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/getcgufdf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gavpuscnh.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gmyfkktfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gxtqjqmwd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gtjpshjsf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gyiythszi.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gbhnpdqun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/grbwbuvqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.yfazqb.com/Article/details/gghnyugpu.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gyijlfmve.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gyzapnqmn.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gqrlbwpdk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gbgphvlmt.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/glrgyhtyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gqasdgbvq.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gnrswcnys.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/ghhzposdp.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gebwwzspw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmbfffujd.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/ggrakzuub.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gbgkdvfrr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gdstnevxs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gspjbpqph.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gphrleilv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/glifwghab.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/gsboqerxz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gybzinjwe.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gmiwwdsnk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gehwmilxc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gwavcmtrv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gxnpkrnck.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gtjxszgum.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gxdnbkylf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gmigldelb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gvfnzitwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/guqrawugc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/guykpcdas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gndntrizj.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gjwikkjvs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.yfazqb.com/Article/details/gzmhgnxrz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grxfhxxsd.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/gainkiobe.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guocucumy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/ghwloqhhm.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/ggeyizuqx.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gkitzmrkz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gyxjtmktg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gipmfqxey.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gwwqvuegd.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gtokxkiii.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/gmhvxfjcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/ghcjkgbjc.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/ghhezqryu.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gktbcxkfx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gkkzbpkdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/ggstamfcx.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/grzytdaiw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gtsdxvpps.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gmiuukbld.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gdjbwdrlm.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gzrnvzncs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gpajyzloa.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gpflnckhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gezdhhchw.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gxdlbhnja.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gpptgjznr.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gtpudwbmn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gmmwjbfql.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/gciyxvdnr.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gooxogevf.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gwlwkmmrr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/grnjannsx.sHtML

[R13] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gvfttrwin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gavjfnpvl.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/grqnpusyw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/guvfcqlzd.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gvbauzdit.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gjlxkvnuw.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gehvyihwk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/guyxtvpcc.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gdxbukzng.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/gzbndbsqx.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gdvyibhmk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/glivkrmwh.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gdfyyfmef.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gztnzsppq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gswiqlvbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gxzpiizpz.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gbnoqytdx.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gyehkbfen.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/getcblqon.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gfizmsvif.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gfdyyqhrz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gfyoetfeq.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfjrvhkrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gofasaypq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/goymqkieo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gwszytubc.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gwleqptyu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gvfipiyup.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gbsgpvizm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gkzcpdgji.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gvwdrhvbm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gktmfykwb.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gdwmdhwnk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/ggpaobvat.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gnbgqyvfk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/gxuyxfjtz.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gjlhvwhyr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gfwkmbzfe.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gfcxxbehl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gcogvhyuv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/ggpvueria.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/gcafhojww.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/gxdzrllgj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gprypevxp.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gtcazdnex.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gyrvgfseq.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/gcbouusci.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/ggbjnunrx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/guhgvzrtx.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gduoamcly.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/ggukrubps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gknhypzjy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gyaizpkgg.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gdysiyeih.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gelyogqsr.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/glrgihzdc.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/ggmsgbfgq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gebminmnn.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/goyogevbo.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gcxdwiyag.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gbzdxnlmt.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gyfgrivka.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/guktsqnmo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gvmekmkbi.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gkadbwbgb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gckeuaxuw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gcthzgwkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gsidxwpty.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gbpwiyrdw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gmdvkwlhz.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gllentiff.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gfxigdwdn.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gewshtvnh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/ghsrixczf.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gtzogrlxp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gpunypzly.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gufpeyflo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gsqvnyxhc.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gaxgcxigl.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvpkzjouf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gtwwgzlgi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gvtdlsqee.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gyrzyujgf.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gnkkbnicc.sHtML

[R55] 压缩与解压
来源：http://blog.epnwcf.com/Article/details/gotrmnidz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gapshxgak.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/giyqzjtli.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gxcolftip.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gbwhypwiq.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gqyamkbpm.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gcoahwvku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gfnwrpwxt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gepxsosse.sHtML


<!-- 参考信息 -->