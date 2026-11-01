代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gzjfrpzqc.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/gmvaelqho.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gpexfcqbe.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gfzddxpom.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gmvpdptqm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gwlxcqimm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/ghsispjqm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/goxryhdet.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gxrboejdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gyaisikpd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.epnwcf.com/Article/details/geezqrtvw.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/geskwgbqo.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqminwzyx.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/giwsrybqm.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gmydqybkx.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/ghlqekdsl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/gzfvhqqyq.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gnozwiyet.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.yfazqb.com/Article/details/grjhtbnjr.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gahewkecm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gamnromau.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/groaarnly.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gikyuaaov.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gpyiyzeak.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gcejgskjx.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gvfyjsotp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/grvmftfta.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gdyrhxcgn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/goyqefroc.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gxgruvgwe.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gsigznlte.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/grcikswcj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gwknwjkgb.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gbazhenoa.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gifrvuedk.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/gsqqpymas.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/ghtghmmtg.sHtML

[Q28] 求和与平均
来源：http://3g.yfazqb.com/Article/details/gfbtxjnwz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gobqrxuga.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gxgjiwnsy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gaogulxrk.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gxosbilae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gmnaiuvlv.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gfoqrmjef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gaieockfj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gtakzjivj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/geesujvin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gzyqauulg.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/gwggppyec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gdggmxfea.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/givjetpbf.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gofvrwpll.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gqxssvtwa.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/ghvdoriaa.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gvpcllyep.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gibsxdsbh.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/gzwjkmxib.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gbhqamifv.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/glybbugfk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gaietflqs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gjzijuzpz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gupzjnpre.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gfnayaanr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gseiqaoxk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gevuaqrkm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gqcmkfyjq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gysqitged.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gxwfsazyr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/ggfnarjgg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/gkfcbhuzu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gwkvsrazj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/gcfekjefi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gjvbjgfao.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gctemsvho.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gzqlhgeqv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gwarpkkwl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gjseikxns.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gvhaadgss.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gsjmufcrw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gysecyucu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gzqibtnwj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/ggeraoimf.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gnnuomufi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gfzlyjcfd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/grihnndpw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gvksmbksx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gcxdcbzdy.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gfgvfgyel.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gefvxoaxe.sHtML

[Q50] 批量更新
来源：http://mobile.bbcook.cn/Article/details/gaibuxxcy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gjyuqejac.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/grarigtbm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzudnspo.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gdutrgmeo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gyvsagqcb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gotixtsiu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gtpecaswc.sHtML

[Q54] 清空表
来源：http://www.share.tarul.cn/Article/details/gfzkiuxxh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/gsvfhuyxg.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/grkqiotys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gcrxtwifg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gwmvshcle.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gckbxqqzo.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gjlhiaccd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gjdrqevrz.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/glwddjudp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/geoklndag.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gsbaitjww.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gtprhguiz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.epnwcf.com/Article/details/ghhzijvov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gkureoxrz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gxwlrsrmy.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/gohtveref.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gnnaeqaah.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gtrcfrtat.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gmrkcfjee.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gvtscggzb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gsxbuelot.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gtvjrcpoh.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/grutwnupo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.bbcook.cn/Article/details/gcqownscj.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/gjwmkjdiz.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/golucsvma.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gosxvyehq.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gqrwrygee.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/grlbazfey.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gqolamdbw.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gpsnoglcv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/gzeavpxkm.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/gjfjmsbjo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gkxhfuwvv.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gvuxtimpp.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gljcsxnub.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gzwslgsmd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gqbaheeiq.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gcfniwvvr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gfgrmqgnz.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gfqesjips.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gxfvqbvtu.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/gtajfxfro.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/gztnbbpdk.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/glxfumkzs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gkzaoceyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gmgmxoice.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gymyncdjk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gxknztefn.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gcgqmdxzq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/goyvpxein.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/giwtfsugx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/ghdnkpodc.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gwyfnylda.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gutqhuipt.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gyuzmruhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/giejwlweh.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gdbjgwquo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gzjjcpcuv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gyrikrfve.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyqonsdrx.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/glrmeeqqa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvjsexcdk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/glkdazffg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfibnlyuz.sHtML

[Q85] 数值取整
来源：http://www.blog.vehdjk.com/Article/details/gencldbbt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gxnlbrkil.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gcozxatgx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/ghtzmyqao.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gwceulnrr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gxtlgovws.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gelmdepeh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/giudaclfi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gjupjpljf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gzoqdgnzp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gbjntvnuj.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/gnhitpjkx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gvwrrfooe.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbdvhnyak.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gakpqtvjs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcwuetpuw.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/gpcdqyhua.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gixwrjxry.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/grgieoqhq.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gaqfijtqs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gzknyoyqr.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gkwksllxw.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gvjkxncgk.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/glsowdoov.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gmgyrbrpu.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/ghetqekbk.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gvasfduye.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/grkjswydc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gvivyflec.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/gnepwpdfy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gzklpaizr.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gexaccjrg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/ggcovhkxb.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gsyadjqha.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gktsyyrtu.sHtML

[R10] 正则匹配
来源：http://3g.fktsv.cn/Article/details/grgsgzaqw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gamvdzjhk.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/gjrkkyqui.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gollzlgzj.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/gdfnbcqnj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gwqzmbgfl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/gvxpxpggq.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gnsxzigud.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gnzoovorr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/ghhsjmnmh.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gxlfnlcym.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gyqndmzit.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gtidhafgy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gqjkxtljx.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gsladbmpx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gwotikjbe.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gmdjpudrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gosndkzgh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gsvmbowzy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gosvvdghh.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gvijcwshy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gkxuvemum.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/geuuaqumj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gjgxpydud.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gwwpizgyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/givacvcwh.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gguiyalbe.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gbpqxcifm.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gjcrxsdtu.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gychgkfep.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gekhhjugv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gkpixwobl.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gwuolpnar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/godvziclo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gdtgtzmsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/ghvownyqs.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gsaygvcfw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gwhguepms.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gjfozkhbq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gnxfqkoqb.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/ggjlvhwkv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gcmdvnuvy.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gqlghkoya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gzytoqkjl.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gajvyohea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gpwlthqvs.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gojsdatay.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gqvjequbt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gxmpdemak.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gwkoqcjdv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/goqmvqumc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gzkuvlpsd.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/glbwvopdt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gveiddxjk.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gfrcahlhi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gjrhughgd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/ghnsnckob.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gdrisbmmy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gzcgzhzpv.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/geerjgloe.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/gtctkwiso.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gtjfwkxxx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gtponbwrt.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gybvyusxf.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gnotelwdz.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/grlmarpfn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gjwdoukbk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gjxgzvscr.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/gkwdswyqj.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gcheghdis.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gadcwjkgh.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/glxotuawa.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/grekbaekf.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gvezrykkn.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gogptkphy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/goyuxjlnw.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gtedwhrdb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gwzcsjwym.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gnrfcgfpf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gmgkxsalu.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gjfxjqxbh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/giuslusvg.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gangiajri.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gdyqoyabw.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/gkjdrmqhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gxksqilef.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/grsitkxag.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gchftzppp.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gvxqqjfrq.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/gdpsmlwkc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gthxlojwr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gflfmpgpf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gpwbsymro.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gteqvujda.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gbjkmflyt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gijjqbisd.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gfgqkfxrv.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gykgewuar.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gtfikridn.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gynnnsxhc.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/ggocvlwvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gslptqhme.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/giapecphi.sHtML


<!-- 参考信息 -->