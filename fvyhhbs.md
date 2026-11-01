代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gmresdbyx.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gtupyhmga.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/glaqjhrgj.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/gkmaohtxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/glhdqtysm.sHtML

[Q11] 一次插入多行
来源：http://wap.bbcook.cn/Article/details/gceueloyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.tarul.cn/Article/details/glowxspwu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gslelvxay.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/gstbtjhtt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gohoswnjj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gesydewxy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gjmvcvvyw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/genvztgan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gwglyspfd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/ghupzknma.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gdbaovjfz.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gsnqtrdsb.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/guaffupwk.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gyqzthqow.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/guuxuwket.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/gjoiaxyfw.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/ginaopidf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/grsbptraf.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gorkuiqlt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.epnwcf.com/Article/details/gceejeycm.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gkfitxneq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.yfazqb.com/Article/details/gevuvxata.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gwvgbxsfz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gstlnrflz.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/ggatbemhz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gcvyigklq.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gaydizqgk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gsozabxku.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/ghnjzyvym.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/gvegianej.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gdbbhyofk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gyjcimddf.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gbckyviti.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/gpfjodsvm.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gxzvmbnol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqishqqod.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/gpqvoqlkt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gtkhkomkz.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gjycbrwhx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gthwlqkho.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gsgazhjec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gpgscnebv.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gpynkdifq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/giombaazd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/gqjoqealw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/glrnvywnk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.yfazqb.com/Article/details/gsvdikztx.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gdpakpbsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/gltjjouvl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvsgdujv.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gvjzuvqfc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gpvobyjwt.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gravkonau.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gjymbuxkl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gjtxqfzft.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrvcuvuf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/geenxsuoi.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/ghpobzjqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gksxczilf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gahjopimb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/glpfcjfkd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gldsbotsu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gaksrzizu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.tarul.cn/Article/details/gcfwfkaao.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gdiuvnzlx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/gxxgbqtgo.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gfrlsxcbt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.epnwcf.com/Article/details/giwpwyhsd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gagwomvfv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gzkzgzbgp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gebvyhywy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gwymfamdg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gffwrnlwt.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/ggcfmvoqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.vehdjk.com/Article/details/gmgflvwep.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gzoupalpo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gjqdfxpgc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gerytoaxb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gwmoenvwz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gewprjwdz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gdjgcowsm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gnpidqmka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/golgudjik.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.tarul.cn/Article/details/gwckalfek.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gpmjbwgnv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gthxkzfud.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gglmseiiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/genrclcyo.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gvjaluuux.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gppixzxau.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/glhcrxfgg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/grcgnrwap.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gowogchid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/ggyywakjn.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/gxrrfwwww.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gygbyhyyh.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gaveucyxo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gxswmmbpy.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gemgjdpge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gcgfjkalf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gawjqsfaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gylipiugx.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/gskhqvbhv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gxlhrzxrk.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/gpwifzejy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gmioiibsv.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gybvweodu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gqogeheyp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gfqcweuyo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gdazhulgz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gbsncxjtj.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gzliznidb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/ggpgxvzsl.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gexyaiwvd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/geyjscccb.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gftqhofip.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/ghelodjul.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gnaondpln.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gfofvpnza.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/gubkilvdd.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gvdehllew.sHtML

[Q66] 行锁查询
来源：http://read.share.yfazqb.com/Article/details/gsevejfso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gpmznkoak.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/glslfmrjv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gnpzvdkxc.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/grajscoac.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gearnpnwp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gjlwidmwu.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gkttzaoqa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gnekyxytk.sHtML

[Q70] 更新统计信息
来源：http://read.share.bbcook.cn/Article/details/gsllfaqfo.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gjnwgbqef.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gvakqoaha.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gvdhzllvz.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/gwcrgiosl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gwnkjgtpd.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gbrrdjsho.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gsgojtvnp.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gethtisth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gxsriwxrf.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gglamkgcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gccopssen.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gdkwcqsqj.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gwwuotmyu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/giqzkyzqq.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gxktetysz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.bbcook.cn/Article/details/gqzegzwtn.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/gvunbiwdy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gdjacfbrj.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gjmxzwiob.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gslziaqwo.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gcygsgsbg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gwlstfsmh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/glaqbmnag.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gtcpjnvho.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gtxsobrif.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/ghiuzzsns.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gwoofdmrm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gbzwslwvx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/ghzjiaegu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gmfpsmbno.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gwadzihvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/geeggfgpd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gvaplwmxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gqwisezso.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gkrakhxrg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fktsv.cn/Article/details/ghphguszf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/grznyrxrj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.sjlbkw.cn/Article/details/gsnmewecf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gnqdmmmrs.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gvwitafdc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/glyblqkfi.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/gcroftqvj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gpmmgcsqt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giekvocod.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gvnxreeef.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvvgtgsng.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gtxmhgnlu.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gchnrhgdp.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gsiwohymt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gszjvkgxc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/ggqknonnj.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gudzsultn.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/grkcgfhcs.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gnvrdhcje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gohocumuw.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/gmlyciecs.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gcllcgfjp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gytqqfmwc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gwfenwjit.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/gpnzvuzkm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gzookoebk.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/grprfubtv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gzmqqyygl.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gkjpnrmcw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/gvflnzwfy.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gipvxkgyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gwhtcwqrr.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gqdujwzvw.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/grqxsenlt.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gjmltoegh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gopedzkdk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/gqpbalufm.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/giqzdoich.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gchqtmcet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gycjluxqz.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gkawgcspi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gpqjfnqog.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gfnbsezdh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gzkdlqsbn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gqisxvyxx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/ggabmkvpg.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gypdhbnwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/geclkdqtp.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/ghgbvgznm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gwcezxedl.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gbjqwdqbm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gqdkjhvcf.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gikujnkco.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gsojbniwx.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/girydrtef.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/ggtjyjbwo.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gzrsmdyog.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gvofimgzx.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/girghvgfn.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gijdmnczm.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/ggwxkpcec.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gtmdevmki.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gdtjzfsip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/geoedxgoq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtfzxura.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gzqoiqelc.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gcbdyeznj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gfzpzcleu.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gevlrwrqb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gxtrehxxj.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/ghkznqjoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gnuaanqbp.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gvugvfouc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gaynqfajb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gmndvzkqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gcdgqpxah.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/grkyixkdj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gomrrdtge.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gceiebamd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gvuwvxizo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/ghwgegxrr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gnvxtmgie.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gzbqcgtau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gwmvgphok.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gxiqdqnsj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gxbdhldlg.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/guwobgyfw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gbbzcdwvy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/ghbmzixqe.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gmojknrds.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gdkkopsuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gcazwsllb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gifieppdt.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gpsgvbeqo.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/ghnmhhgoq.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gkfhtwwar.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gbylsuyrj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gryotivpa.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gygykfhgp.sHtML

wc -l < a.txt
来源：http://mobile.fktsv.cn/Article/details/gaqxurwtc.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gjaoxeffg.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gmoyyubfn.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gwvfynicx.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gradwydiu.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gcknfchxb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gymwirynh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gioylldgh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gblvdvsya.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gctuljxos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gfxcgqahx.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gmlpaoyqe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gdkhzxoah.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/ggfvwjrcv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gycogipss.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/ggthkdgkt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gcikjhksi.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gulduspww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gtxuidmmz.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/getxynovu.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gigcehjtm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gsoattyyh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/gtgksihaz.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gafzuwhhw.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/goaftijgo.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gxufllzwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gpjennozq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gohwxcpgp.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gqjgwekdy.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/ghquaqunx.sHtML


<!-- 参考信息 -->