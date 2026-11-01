代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gewsrdazq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gvdykrkki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gkgzqcptd.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gnnzcqeea.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/guaotbwro.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gakoykdly.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gpoejmemp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgvqbgtw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/giowkhquv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gikkiylck.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gxwmzamtm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gvrbxytod.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/gvajlbepb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/ggrcpnczr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gmhursgll.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/guzunvozw.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gztcbkmah.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gvkwkusgm.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gxemugcup.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/gzedczxwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gmwvuigyb.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gbkxaxejj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gcvijzyng.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gxpmbukpy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/grpzqcqzw.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gabqafyma.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/giefegpmm.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gjbfuxowg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gxahhuiuv.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gcikmswhr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/giuobfshx.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gnzaalbtm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/guocaolhb.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gcupgspsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gmsgohvxq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gbrfzfnei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcfholut.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/guolrbrmw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvquhywlj.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gwkjiimoq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fktsv.cn/Article/details/ggbqmrfxe.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/guptbtpso.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gpftzxtcl.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/grpfxixbx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gwhjuavqj.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gcaubvlmz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gnobybxqg.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gytwiogkp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fktsv.cn/Article/details/ganukiykg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gciurjbzp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gwwkaojow.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/gruasxwke.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/ggssukqsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/glqzcdgfl.sHtML

[Q34] 每组取第一条
来源：http://baike.sjlbkw.cn/Article/details/gdhtxbvtx.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gddejehkk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gssozubdu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gpafdrocm.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gtevgkvqn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gocffkmpd.sHtML

[Q36] 左连接
来源：http://mobile.bbcook.cn/Article/details/glwlgmgfy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gluvvqzpt.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gqxgmssvf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gmzvxjzru.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gmdxpnrfo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gvbbijent.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/gqhiqtkum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gpyvqfgyd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gtwmgxtoo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gdeybmace.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gwiglgnpg.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxhxepho.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gbqmiezlt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gkchegyrt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gustzfbub.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gestzstgj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gysjtcobj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/glqqrhkar.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gqoxjmgll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gesuulpzt.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/gnsczofso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gijbyzwkl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gpvdzhzcg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gwsdlghya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/ghhxdfubk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/ghuuxxrvz.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gjqhecwok.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gtnatecua.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/giyikblvd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gimplfndi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gjwssuljc.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gkslqyyfh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gtkwobtek.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gcdhnksty.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gxwjopnaj.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gsrxudccf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gsxwedclb.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gzbprjuwx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gmebplnll.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/guuenwiyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/ggruevykv.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gwttiohzl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gzcylnqnm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/glvuyotqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gkmaazgbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gfjxbnhzc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gdujglbsv.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gzovnnxzk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/gvdyhxhlx.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/ghftsywfk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gyrwsufjn.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gpzxgnazw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gchwecixf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gcnlctgye.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/gnofbgkbr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gvnurrlfg.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gjexrwwgx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gagqciejc.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gzozwxcks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gzuddvtle.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gvvflrwbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gogxedwyv.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gnhtwsflg.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gkoqvvwbw.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gxgnggyoh.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gueirdhyp.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gsdrxtiuh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gvzctfrpc.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gcsvngrar.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gazqwwwkm.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gxaeyqnod.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gcndkawev.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gszamyurf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gtlmhgont.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/glthdkuhz.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/guncupdkl.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/gdsxmxcrt.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/ggekqjdfy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gzncjudhp.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gsveiwzlj.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/geqwuiorr.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/guislrlss.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gjvnqfltr.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/glxxifbnm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/gbumwdext.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gbljemeot.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gzcpvtwxz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gchaqroxj.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/gkmlywrac.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gtebetamz.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gxdigsbed.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gyuarjxdb.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gdkeidfde.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gbuvsfqjz.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gqztmoput.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gmqomepyq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gjxrdrrkt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gcypcfupg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gfbjiudxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/ggeydbhmm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/gwdylskpk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gpvabjqgq.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gyqwnpirg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggabqifga.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/glghqliwx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gulwzegab.sHtML

[Q85] 数值取整
来源：http://read.share.vehdjk.com/Article/details/gdknpecwu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gnvbhngoo.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/giflnhevj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gijkleqff.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnvlxgmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/goyauucqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gpexufxpk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gxwnnjzpq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gipovhvoh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/geykosqrw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gidzjkixg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/guilfxfhx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/giwavurtp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gneqlrdkv.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gqtqiyxwv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goqunzawx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gaznypmgr.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gbmqedjlu.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gjzkqbtxc.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gsaehsxyx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gnjdckvbj.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gbvseqocm.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gateiylja.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gprwffonb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/gfcgyhbak.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gyazacdua.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gpzxxcgei.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gukmckljt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gcgzlxrwv.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gldbgesyb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gkzjuethy.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gdaslifmd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gykqpkihe.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gtnutsjjk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/glapfupfa.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/ggddirjow.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gyvmcwbor.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gpraurzip.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gxjlkhmfx.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gigrvlhwq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gkjycggpm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gvhnitkrf.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gqaszrkvs.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/ghyaixbpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gtevpdoyj.sHtML

[R13] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/guyptffja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvalntrfx.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/gmdpxwsij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gtoricqpf.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gcmdbmnod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gslcqzneg.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/guucafdmq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gvmkandcd.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gnvqqoife.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gdjvnamdx.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gpcngykmc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gqlwxoyyr.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gnhtcraah.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gylrbkbvq.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gdpdmptdh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gywzhuhqm.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gsywyidig.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/ggjdatslt.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/glgwymdwr.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gdncpmmwi.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gubkfflbx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gwhinjgxs.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gyfhphdxe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gzicggmgl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/guotpmwmd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gxkkqrxcu.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gylikhynj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gnbvrfmus.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gbsaqfjuc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gwdwphkdb.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gngamamku.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/gvtsiqrws.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gcmmorlfv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gngxhskdj.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gcjyyffaf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gsbgfveyf.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gticwjjcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gcipfqcdz.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/guzoocoru.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gbnbroofi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gwdxuegyq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gwbwniqtd.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gnszufyeq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gjhamjpvz.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/gcrrpoozw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gvomtgvfc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gmsuugxab.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gpxwcqyku.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gyhoymjsq.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gwmbqdgjb.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gmobcglaq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/guddyjovw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gsikmluyy.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gnheqpgge.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gmgxkjmkq.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gmhtpdnkh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gumbudgmb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gwgyqdjux.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/guqnawdlw.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/ghecexpqm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/ggosesizc.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gkzygnalm.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gltmpgcvt.sHtML

find . -mtime -7 -type f
来源：http://read.share.sjlbkw.cn/Article/details/gbquqqkiu.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gjjqgxkry.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/goaeraxnb.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gbrflynuu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/geguaqcpn.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gbarfdzch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gvkaqknpm.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/ggnniukvk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gyhlzaacr.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/ghmxdcpwp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gfwfyfqqq.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/geyzdksdl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/geyjpbzvv.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/gzeepmocj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.bbcook.cn/Article/details/gnrrpjsrk.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/guhgmenub.sHtML

wc -l a.txt
来源：http://mobile.bbcook.cn/Article/details/gikfosbyb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gbypstsol.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gzaukqpos.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gigtmzhei.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gvbbcrwdy.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gppookugk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gdxrxadsc.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gsclkodqm.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gagwoodiy.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gndxlsjas.sHtML


<!-- 参考信息 -->