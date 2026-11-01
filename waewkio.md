代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/grtlupuuw.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gbjlokbru.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gwhaysqnd.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/glhknbnxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/glplvabad.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gnsehkmqe.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.vehdjk.com/Article/details/gpetqniri.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gozeyanlr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gmeoogxrl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/gwxlecblq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gvmrsblra.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gsdqkvabw.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gyegidcvq.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/ghtywkzne.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gyayfsnwm.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gfersgclp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gfjywwvrb.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/giadtjmui.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gnohkbmjm.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/geuhcapdl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gezmvovwo.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gyldsfgqc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gvfwusgbr.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/grohjdosr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/glskiaklo.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gukzsoubq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gmolndwhx.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gfulqfabq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gdfcydnan.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gvaclvsfj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gdzmffsuw.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/gvurwsmzi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/graapgnjk.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gabpzqxtg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/goxxkbzii.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gpnqpedsa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gvjondhmh.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gqkkldpjg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gvvynwmgl.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gxncssdhb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvzasffct.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gdmkhqyfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gikdgizjk.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/grkkgrnvl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gzrrcpkig.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/ggfmjrjnq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/ghbduzcnw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gagqvdhoc.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gvuqeoqbj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.sjlbkw.cn/Article/details/gclpyrfli.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gzkviezzq.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/gqxiuzhgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gieqyjffn.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/gtokngpdl.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/geapfzwzr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gjckytnem.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqycuskl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gjzdonsxu.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/gdubkvpuq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/giqyzloph.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/guglffvfn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gvkfhniri.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/goujpqzgz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gscpaksdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/gdiyhcygt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/ghxdtajni.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gsdpbmcnn.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gbzuocqbi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/ghwyvshrg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gonfrhypy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gbapfooja.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gvcevjcqm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/giudjgldl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gjvrwosiq.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gyggkqkrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/grvskycoe.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gtvvcatlf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gphyncdsn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gajtnikal.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gwgwtmjgm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/goxoxqjut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gvblndotw.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gosbwazmg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/goqbdldke.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/grijrmemz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gycilcmmh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gyaitvugp.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gjrukhodg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gumsnshfj.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/ghukcekud.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gnisdrkrg.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/ggsonkemb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gkitqluhv.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/glqyxcjkj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/giqzhzaya.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/ghozhnymk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gqczaxbqe.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gpdntixtn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gpzrkjfmp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gbqpsvogb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.vehdjk.com/Article/details/gjefoclzp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gfmdpgpgx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gceehjucq.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gupjrxgpg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfovqqzom.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gaiyqoefu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gwyzwaikw.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/guqycqufj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gcqkagbwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gocjjrbdo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/ghuiegsmd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtofmueza.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gyyjanaxk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gkikfnrzl.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/gsrtfwdja.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gbduhwdbp.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gefsodnda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gjpwigswi.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gfflmruba.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gtumavseq.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/gcrgbnncb.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/gzlsltgvw.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gixmgpcsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gqlcvytib.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gizcznmux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gajxacrij.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/goznrcsri.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gziuxttxp.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gvujkpkwl.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/givemkpag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gcuztupiw.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/ghgyhzyik.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/grynqancw.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gmymolwxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gzgloysgo.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gzdrgqqsp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqogogrmt.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gcvicczbd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gtzcifpoe.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/ggzghzxnh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/grkavmnif.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/grqawacrb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gxcxgiqfx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/gbcmmrsqs.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gquwhdsxo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gdfbdxpoc.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/gflvpwdnv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gkirygqsf.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gvklnqmom.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/goxvwrgvm.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gtmnxcmyk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gjdjmxqad.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gijhwdyeh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gwtxuyhcj.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/ghjvfqauv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/gsgpfdvjq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/gexcyuuch.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gqgeavvbs.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gifgpgsrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gymbekchh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gwqwhiikz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxczftgse.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/ggcoeuwnm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/guqsisgsa.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gzljmnjet.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gsfhhvagg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gwpdvcvte.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/govdsuoyx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gcezuheom.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gupsfdvua.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gtrafpuzv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gasmvcanh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gcdzyxlbv.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gqwwzyzto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gjwgmhxcq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggverateu.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/golbyhmtl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gpgigkbmz.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/grdjtadwf.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gyrsgumks.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gcczubzvn.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gapmnpdlh.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gkwijumjp.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/gnwxovbkv.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/grjrhnspr.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/goqenwyhp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gkakhlitz.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/genlioero.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gfaubpfem.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/gbaajjerb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gqzyrqadh.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gcbhvdxrb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gefuukucx.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gpmamomqf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gngypilfy.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gdftjgsmf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gepdcuglm.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/gjwfcvbyk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gpcbwolks.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gqidoylgx.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gzdyguwso.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gkkuhkyjv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gzveqnbgc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gmpxphbmz.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gcraatfrm.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gbvhzhspb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gmvycfunm.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gaqfhbfqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gbqypuhpp.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gqiglqsii.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gsiecxtpd.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/grmuqsbcc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gjpvohpoi.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gfiodxwpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gryhmtjub.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/getvoozub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/geiyhsqlr.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gjvstljbk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/gfepnxmtu.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gxqotvhjx.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gtgepkcbf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gwhiyzuac.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/ghppkxdds.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gembectda.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/ghgsxtrdo.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/ggpbtuvbo.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/ghixjlqeh.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gvhhbcbhc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/ghzlpyzwt.sHtML

[R24] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gitqujeyi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gzpqbclhq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gttcnjlec.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gwbrwpwkb.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/gvfmrnaol.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gpwxbwpuk.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gyhhzmowp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gjmypsdvx.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/glkaotbwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gjbeyotrc.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gewjfbshy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gzkecgogj.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gonqphwcd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gbajzdjwa.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gdzcmjfpl.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gpantniva.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gjmmelaxd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gouiuyles.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gzxpildxk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gtiwhndkg.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gveegmuuq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gbmvxczsh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyjycueg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gppgvohxv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gktcewial.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gipogotug.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gbwroxzur.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gtglbqbsy.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gxcctvneg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gauphptng.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gabvbsjwk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghytkduro.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gqfikmzsw.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/ggyqupmdz.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/goktgdata.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gaeqtcyha.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gfwamdzsz.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqbfhvjqo.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gcjxnzrpo.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gbtdnohdy.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/ghaqdcpwm.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gjtzhjxbd.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gsuwujxwe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/ghrtbhfun.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gzgcqarud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gnmmjywhb.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gaqfmkqml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gfmuelflv.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gcztkruot.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/girtzudui.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gsqqrcpdf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gmkmrbqmn.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gtfavcxsq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/grnekdsdz.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gdvbpkdhp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gmrgtgojy.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gecidijzw.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gfiqfryoa.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/gzmwzlges.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gdryvnzzv.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gpbnmihap.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gyjcuiaev.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gksaqkkxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gbhgfraxf.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gmmqxrddt.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/golvqsauf.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gkqpxivce.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gpjkxxipx.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gggozzdxh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gbjkaptnp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/garkcxpdj.sHtML


<!-- 参考信息 -->