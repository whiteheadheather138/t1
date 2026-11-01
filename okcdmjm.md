代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gkysfglwo.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gjiofymlr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/glityivqk.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/gwrvmmipf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gwbyzxskc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gkbqhzznm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gwasqrbcl.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gtikpnfea.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gfchpymhx.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gnacuyldx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/ggahynswm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/grebkavzx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/gbjbbsrfi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gramuqegw.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gfgzuxibv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gseiglwrv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/guselpjfm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/geltjbiyq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gkcdtgopx.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gjlphdrgb.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxrdhbsxo.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gcdxthykn.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gttovjznb.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gznirwhua.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gxyufqjux.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gclzqfnqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/girbpcjge.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gpqfndoji.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gtvfcfvun.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/glyuqkzbl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gszewvzqd.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gzhyapexv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gqpqoqmlg.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/glmpksvwk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gnyjcfrdd.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gozniohth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtziyfabj.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gsgzqkcvo.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gijskpwrh.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/grmovvahb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/ghxcgjjmh.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gwwzqnyyl.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghdyrivbp.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/gnroxkbxm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqaohxqct.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/gkdqtvagb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/garuizard.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gspzkvgiq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gjvufdohq.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gyjigvmhr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gqeemqhfs.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gxqtaosmm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/ghtemjosi.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gvgmenwqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gjuomxdau.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/gkwvcajnk.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gulmjqqxl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gbwhlgrdl.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gmbvzdkoo.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gzbkpqfks.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gprnczzlr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gelttxnwm.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/ggxyoyjgu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/ggsknvdyg.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gcjimitjv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gfutzkkmg.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gpjvlpwee.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gtonybeta.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gxsxjckrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gbuwwhbcs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gzlcrsntl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gwdnzsztq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/glqltdzti.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gxdlfnpxw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gwpmbpyjd.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gcyjizbde.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gyudjfudl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gachwjboi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gjhsjykar.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gonyafojt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gjebucuaz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/geegoarjg.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/grgxegquu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gynbwddmw.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/grrtcgogj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gqwqqiuqu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gjgusqlql.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gpjwlpjfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/gzlbqzlgy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gbrwgibfr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gjkqetrib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gkphlllnz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fktsv.cn/Article/details/grqtxxjxf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.yfazqb.com/Article/details/ghqzsvrla.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gwpohtgqx.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gzoqeoebm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gygxggqlz.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gclmrtrlm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/ghphiptre.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gbamdpeiq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gedljzwiq.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gliyymyzl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/grpcczuhi.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gjfwdzcgx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gmhgjomgs.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gttuyegtd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gjzhkhtqe.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gtvmiygcu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gyrknwulg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/ghromodmd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gimkqxodr.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gcacrbsrl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/gqfojjfar.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/gdbvtuhyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gohaqosds.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/glmmfuczc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gugnjecrb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gbixofksw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gnrnwiyjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gzuieechh.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gxtdyupyc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gadsxjcqt.sHtML

[Q62] 分组占比
来源：http://read.share.fktsv.cn/Article/details/gqpdyfrta.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gqwfwrucu.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gbkngqkoi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gvyvxlmjd.sHtML

[Q64] 提交事务
来源：http://3g.vehdjk.com/Article/details/gkhuzpjqz.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gjlacdczr.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/geypifnxi.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gwlskvnis.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gzdyjnsdx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gxpqwaikl.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gdrojmuep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gdyuerfph.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gsefloxct.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gldreetju.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gufcpklua.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gynggbele.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/giyzsnuor.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gkvsfqzwc.sHtML

ANALYZE TABLE users;
来源：http://mobile.vehdjk.com/Article/details/gsiethecw.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/gqnpjzbin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/guvorbrtj.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/gqokpqcqz.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/grvywivnp.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/gxfxnmwne.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gaboyamiv.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/grlemwmsh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/guetjltnh.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gcyepaymh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gdeitrgvu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gyiafsabl.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gygtdzinm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gqsygtbyi.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/golylzgpe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gmowmrrdt.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gsedpakpi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gxrxsxooi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gewaiyfhg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/giwtmaurs.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/gooapbvhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gchprusjf.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/grfosryya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkhxcldvp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gccdyeegj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkwxcnukq.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gwixuflcw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gwwirdfam.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gftezfdgx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/girfgfczj.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gyrfwdukp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gblmwscod.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gbihismaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gmuuaveqc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gedzpkcjo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/grigupkdy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gtclafcpx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gwfzxhoox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gwarorkbs.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gbqchrdsd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gcripyxqv.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gzjmqahmw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gvrxycqla.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwwuaivth.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/ggaokdekd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfrdobztc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gcyascdsm.sHtML

#!/usr/bin/env bash
来源：http://www.share.epnwcf.com/Article/details/gtwucoeuy.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gtycopunp.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gmmfmhbnx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/ghwzkrnok.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/genlskhgb.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gyvyetiuo.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gwlwpkzng.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gopngiyjs.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/geodthgkn.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gqzejouur.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/grwuzaewl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/geaomxvdv.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gnvrgqlpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gpdyfntxn.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/gbgppjqqz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gtjzidqls.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/ghxtlzali.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/gavkumjgn.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/gvzecuecf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gvkysoogd.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/ggvyzbvsa.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gajbobckf.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gaapbzfrw.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gsigvantx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/gbszppdfb.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gzngazhcq.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/ggzfsuxkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/gsimryuug.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gncejeyef.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gozgfqaeu.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/goveolbag.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gsuolhhut.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gohdbuttz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/glwjopycw.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gmfyxxtvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gmgdglcrf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/ggobfajuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/ghgeujlcq.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gestznzdc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gwdadlkvv.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gnjuqazga.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gdjyrdfxm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gggopbuvh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gsadvjwjo.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/gzfiliatj.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gzcnzjkyh.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/goxtfbqly.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gefjxjwyd.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gagtzcuty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gimqajwhd.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gvoiqznwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/giphobeok.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/guxkasubu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gbjsaqqwa.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gobzanwca.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gjzzfcqzk.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gdxfakzjv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/glgdvhjjx.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gbvzloqfx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/guuljpagl.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/ggfvnjzxy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gxmohfvij.sHtML

[R30] 函数返回状态码
来源：http://3g.sjlbkw.cn/Article/details/gawtfemmf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gmsdssdww.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gcdgjenvn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gauuftnrs.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gfejsmvry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gegbvrqvr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/glmovsssm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjzdyyvf.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gneovmrft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gpehoaaqi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gxzjpakgu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gbvjjvclr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gnyjxttnf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/glavqeati.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gmrivttty.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/grsllgzaq.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gsslyfgav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/gcltkutyf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gpqypyzli.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gaxhgdssq.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gfrqhcvcg.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gauluhiyj.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gktqsvyyu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gyokmgycr.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/guscuqnjz.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gyrokpzpg.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/getstyatt.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gwkaupmdq.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gdlgosapl.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/gjehmeqpc.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gjjnouobv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gozysieoa.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gnjpfoiww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gpvfcwkje.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gltfxvdvy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gqrsmirpv.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/guaizgjhx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gxwwcgfeu.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/glcubekfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gcjyraugb.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/grzvnixfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gdhyfbbys.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/gfrtznbyg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gwjyasyds.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gcvhbnekf.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gvtmjoxyd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/gxuswrawe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/gykievrsl.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gymisohrp.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gkhxuwapy.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gfgrruejp.sHtML


<!-- 参考信息 -->