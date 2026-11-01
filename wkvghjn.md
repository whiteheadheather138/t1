代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gbhvutrll.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gkspnsoqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gmsmnmlpc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gbmsolnpq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gqzboxijh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gerubmojd.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gaetlohfi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gbsljqmvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gmvbbqhkr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gokpnuaoa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gcddjlprs.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgbadfva.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzrebxaia.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gqgzqkvfp.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gkhihrlsv.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/gfswwkgeb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gsxeeniya.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/geaynrfws.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gjvwlxgxj.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gtiymfhxq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gjjmbtmry.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gwtsfrvwl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/goozcwngk.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gfzstommo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gwurgbiev.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/ghqjkozal.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gyxhfvqvq.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gnoitkjrc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gquxaikjf.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gsebvlzrd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gavymngag.sHtML

[Q25] 只取前 N 条
来源：http://baike.epnwcf.com/Article/details/gowvxxktk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.sjlbkw.cn/Article/details/gdlicaclu.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gjsywchns.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gxairyhts.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gsvsnlszf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzwwooeam.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/ggpowidtk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/geuvnldli.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/ghckyudco.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gojxvelxz.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/grzdfgjro.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gfcsrfktz.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/ggadxiehl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gwvtxxnnf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/gqpmzktqd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gmvnzwpji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gtpcppphj.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gynycfffs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/ghihxbfba.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/gzdagbghu.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gpdmwceyc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gljhoxygl.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gwvhjgywi.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gknkqpzam.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gtmzxancx.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gskfwltsu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gdcvabmac.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gaphekgjl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/ggwroxihh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gbvqnwjrc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/gxdobbrml.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gqheonqua.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gfnmszwss.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gwccfgotq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gkbbkebmp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gdnvgvork.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gqqdlpwmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/guqjvovxr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gvgdhmisg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/gwbiskxzj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/ggoxpukkm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gekjbvjjf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gcellrlhl.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gmgdmewog.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gguyweckn.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gsbvhoehk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/giiyxhiyr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/ghdwnrcyg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/ghqpgdrjb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gvvfiqwll.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gbbashviy.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gioppdrsw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gjlhtdjny.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/ggljagcid.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gevjbyzjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gfcdpdbsr.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/ggobwvnkt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gwayuqtsl.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gnuepuxuu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/grwxaptwb.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gnlrikgmw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gkepvipji.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/garayypkk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gyufyzshy.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gaqkavvjm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fktsv.cn/Article/details/gxibkvpky.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gdtskwbau.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gfzewkqgr.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gcqabijct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gmzfxdqkc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gwdmckclt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gthsbilyj.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gqlsoyhrr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gruzuqurr.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gtjtqqnrh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gvzyyjimx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gvdznyvrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gnkxaxujr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gdjbyvyjf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/guiaknhyr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gusxoxlox.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/glmdwplob.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gptssfwvv.sHtML

[Q62] 分组占比
来源：http://m.share.vehdjk.com/Article/details/gmsyxjshk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gwwtanoen.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gcljozpdk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gbnablvmy.sHtML

[Q64] 提交事务
来源：http://3g.yfazqb.com/Article/details/gdkpbmxad.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/giiunecyo.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/gmwrhsvgg.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/ggekctgxt.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gxymkgsli.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gekeixzrs.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gwrjcmjmc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gwfixvfal.sHtML

[Q68] 保存点
来源：http://wap.yfazqb.com/Article/details/ghtouxihp.sHtML

SAVEPOINT sp1;
来源：http://blog.yfazqb.com/Article/details/ggocqyzzk.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gczdcghjo.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/glbvtajit.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gspmlosfl.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gbuvslmov.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gkxnxnrde.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gbjdtdkbp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/gfvdbthpr.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gmpyrxjeg.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxkdqwuvv.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gzjshjrnn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gyytlkeap.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gmdaregkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gniplkaoo.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gqhtiycwa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gzpxgwxto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gmqwtmceg.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gsittkevm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gdmvedgqm.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdlpvyjb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gjwjibcfb.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/goteiqycl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gebxaeahg.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/guhvzsoon.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.bbcook.cn/Article/details/grivmihyu.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gcapffooa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gojgmrffq.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/ggsiiqbek.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gbwqralpt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gpvsutdqf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gsoewqtpr.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gfkpyggiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gkwtpvuyt.sHtML

[Q84] 去除首尾空格
来源：http://m.share.vehdjk.com/Article/details/gqtxcdyng.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbieeqgtc.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gypdcknqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gnnagcqtw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/gufghsjup.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gzccsjacf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gouxytirl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fktsv.cn/Article/details/gcydgykwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gtffeoitp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/golvuyzsn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gwannikte.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gjshsinrk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gfewsxfun.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gfdiuxrti.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gdvvaspmp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/guimjeoqd.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gmwhakrey.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gewjmwkff.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gnkliwyic.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gbqemuxjk.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gzdxizvvg.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/ggeytvnon.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gefqjfhso.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gjenfnpqu.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gfribtybb.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gpycetmdb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/ggnxgdzzb.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/gxowmfzxf.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gguuzpprz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gwhjcoihc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gvwglyaij.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gmofdcehw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gpqgevgfa.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gyaseqnod.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/ghmmgtcod.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/goguxoybv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gdxwmiqbg.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gszsnsytt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gzdkkojhh.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/goizrwtac.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gpvhhphdq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gvkqwyvvc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/grvzzrkum.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/glbhoujde.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gixuiercm.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/gbfovhkxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gsxhpokkb.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gllsorxzb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/guxxjuqsp.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gwgbjdlka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gpqvqgdas.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gwbsyqjee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/ghedkfbir.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gfbkluinj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gewfewyqn.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gryfhojzh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gepycrtld.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gbehyrjxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gyekaksvo.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/goebjtzzy.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gnmqizfwb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gmwrdazfu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gybhpnmho.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gpfyujdrj.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/ggvkgphcb.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gdadvrpak.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gqklafjgv.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gsumvfiqj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gcimxxdcs.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gdrsxqgoi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/gjukpgpqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gmojjtgnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gdsascznl.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gtirlwinl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gvhvliobo.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gjjdkihla.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/guxkofrwb.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gtkvccxry.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gdtooodnb.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/ggtyqngmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gtordeshd.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gfkxvtdhy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gznlekspy.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/glyiofuum.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/grlnnjnzh.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/guoembuvn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gwalnsmbu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gmdfrxoig.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/geannnscc.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gyijagzmt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/glaixducv.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gdxrijniu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gypucyaai.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gqijcocja.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/ghncklvey.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/grffpobqz.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gcjfdbjsc.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gzcdwsumj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/gmychwfye.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gfuuntszc.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gjurvqumy.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/gvvkydegg.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/guaqhxcne.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gjoqbpysr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gdtjfpldr.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gbeqmkzrm.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/gaqeppwwd.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gxwhismhu.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/goymnwpoz.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gkdijxbma.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gadjwspma.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gdonaappb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gcfetqozc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gonwrlalu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gsiiwxqkn.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gbvbpwypr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gmxqwtghk.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gkzmdcevs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxzclkvjd.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gphfgeqvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gxdzkajyk.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gfvjhjcsh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gowslhais.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gufajrcwf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gwwfhfhmh.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/grgrmprip.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gbhjehfsb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gdvxvqhha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/godjvbwwv.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/guurvitbe.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gbwjzzcts.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/gmxyzmkim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/gpvgvqtgq.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gkgovhhlz.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gmnbnwsqa.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/gkwiojokb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gtzepdzkn.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gvsdemxly.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gakskxowh.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gjwbwwbqa.sHtML


<!-- 参考信息 -->