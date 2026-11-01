代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gyabdenqy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gxydpzbjg.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/ghgeldmfo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/grhnhqzre.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gonwbgjnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gniqpvihz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gwuebbzcs.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gwcojzpva.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpnqsvzyh.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gnyqeuyfl.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gddoakqwp.sHtML

[Q17] 条件查询
来源：http://wap.vehdjk.com/Article/details/goykyqxhx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/grujunipk.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/ggvhtdulg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gssimzjgd.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gvihkekiz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gbbokiunc.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gisfgschx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gciodzagv.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/gfttxymma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gkddadtie.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/ghgdhkxpc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gafdtpujt.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/glyuaqcht.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/geswnzfcx.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/giemqdugn.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gaxlbuqqm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gwmimuqqh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gxyuovdng.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gikybofdk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gjwkopsrz.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gtjnrguhx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/groklynnn.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gvbeflhwp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gncjysrrn.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gsnhvvrua.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gzscemxjg.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gsynncvvu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gvqtxigci.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/glwnzozkl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gujfaxgni.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/giwdwzfws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gtadrzalf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gtnyzlsxj.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gsvsnbwnh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/grrxdfksh.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gkxbmgqxk.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/geejhvnie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gxqdltihz.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/getaftgwp.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gswpzuomv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/ginlhzzfj.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/grcbxfsxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gaekjaodc.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gfxouleoq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/ghohsespz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/grtegzexm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gkwgxlucd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gdraapmeg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gzupymsfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/greyoldcb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gsrxfcakf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/gkjejzcct.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gtctydtpm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gpudrjphm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gpeontgwz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gsmvpgqbi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gniliqefj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/gklcvguty.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gxwlwauie.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gwhzwubhx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gplabpksq.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gngwgxmtu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gdavaavmh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gjuuahvvm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gvqkiaxyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gtkpefqsi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gtiasqdsy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gvohwvqgj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/ghloblblm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gclkoxmwe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gkywinqay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gkztttbqm.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/ghfnjqfbs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gkhirfsmm.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/gfsuzmifn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/gugqvnyyo.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/govsvnuqe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/gqhpucyfr.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/ggisjanuy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gtmrxykmv.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gdctmlsmq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/glivjkqvu.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gvymveuqu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/ghbytvrje.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gtnaneblw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gccqcjhpf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gfecwgehf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gdrccedic.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/govxyyaxu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqhtbtcny.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/gqstkiknb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gioqdkgpy.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/ggappxwip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gofwkmjer.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gkwvblvcc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gfqnbodrw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gonnzqzpg.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/godrdscoe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gbundzahf.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/gvufexayr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gnlnbxxod.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gnwheavvp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gbsyerwko.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/ghwhicqml.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gjbwhmhqr.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/grykgfwdm.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gwgnucnjg.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gdoqhvixx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gmdtejbgx.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gaurblsev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/givvssspd.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gkmxpxzax.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gxppfzqmk.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gzbqfwels.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gtbyjrfhi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gpamjmtxd.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gxxbjvzkl.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gudkugpfr.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gewqkwyzs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gjjzegftc.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gzoldteez.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glybhlxmp.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gxjpirhbj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gbuqnlvox.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqkifjps.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/gxiktzvxn.sHtML

[Q75] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gedmexfmu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/grjddipkk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/grvuinuly.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gpciscxyz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/georsxsla.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gkqeqnhrj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/ghiwkxoqy.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/gaypxqiui.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gammltttn.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gkgwuflqz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gjigsjknd.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/grovaqkdu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gngciiqix.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gjqatvsno.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gljoxvzny.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gxsopygxb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/guczxdhrg.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gynebstdi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gfvfrrqbx.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/guyfkabsi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gbbyofzgg.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/gqwnwlfox.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gnlxqclwj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gupxkxehy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gtadwrrqj.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gdljckjui.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/ggptfpgab.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/ghlalehgj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/gluyfpoph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gfilkkpgs.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/guwpbzthf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gfyzikxea.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/galbgodwd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/glkzmrdhc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcffogswj.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gjzwhytir.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghojlisax.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gregjmbhy.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gpygwafyr.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gwcpdmjba.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gtnmqsars.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gmzdmyrlh.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gqjkteqnu.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/ggtkrlzsh.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gmmwboywj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gtgdhjyqp.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/gxgflhjxm.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gdgcqpxft.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gseybqdue.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/glezmjywn.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/gitnrfewu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gxgjczgsi.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gzzuwmnjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gdfyceuxq.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/ggbsthivm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/ggzzrvmca.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ghqapcmup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gfubcdjyk.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gssxcbppi.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/guwnmsdyj.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/giahqoahi.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/glkzghqkb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gcrktquqx.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gflvoxnbp.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gusysnckc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gfqyeajbp.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/geslsvcsf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gcyiviyqb.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gvzrhqtcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gxbljpgyy.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gofnkyood.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gbtqhfhtv.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gxalyclul.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gghhslahx.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gwpkfzbsu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.bbcook.cn/Article/details/gctewxoxd.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/ghudaasxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/glxodehsv.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/gjhvivrlt.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gaahspyze.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/gpynbbrmc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gdxfqsizq.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gofzpbcve.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gjbwmageh.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/giogmmtcs.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gzyiyqhrh.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gwiojsvoh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.vehdjk.com/Article/details/gnqmypwht.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/grunsfugu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gavsqqcjf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gvjfiaqxm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gixvzgfdz.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/gsguxyisb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/glrfivghj.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gctlqaogd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/ggimyosan.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/gdcrevwqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/glqzkljjq.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gnzeayiuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/geedkujov.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gkxypccxm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gieaawotv.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gswxnycoz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/glozccnkr.sHtML

[R32] 参数个数校验
来源：http://read.share.vehdjk.com/Article/details/gfspyiqhu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gmxgwodtz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gnbohmwrk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gjsubuxvc.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gacmvsbnu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/glktgjuhu.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gaiuygdqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/glprgxcnb.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gioqmyxpd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gbgebagca.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/goewgaqwd.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gwozscizg.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gvhmzsgqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/giemjzbxn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gscrkcdsk.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gjbsyfqnv.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/ghnythcar.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gqjjmhrgf.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/grfoiievn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/ghiicqwjz.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gmiptqwzf.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gcolwhofc.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gcdrmvkky.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gjppulffr.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gylbhtgqm.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/gplkccjfp.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/guzxrwyxa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gbkqnjchg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gmknbscpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gnliqgjvo.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/gtoqtqqpi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzzpyvqch.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gumbkoebe.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gwpypaych.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/ghvcthjrd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gvtbmryak.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gdmrbzkbr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gqfcoacyj.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gviyhqayy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gwprfmwgw.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/gwjgikgap.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gzrkrvvff.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/geuezdmkx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gjmudspvp.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gimxnwhmg.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gxbuivdgq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gqmqiavts.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gesgffcyl.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/gcymgvsod.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gmdzsgrhk.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gyxcmwikn.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gopeievyk.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gdimkcwmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/gdjitfpcz.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gtylzlaza.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gloxjlyah.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gyxvrgagb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gmtcmckuf.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gzkhtecie.sHtML


<!-- 参考信息 -->