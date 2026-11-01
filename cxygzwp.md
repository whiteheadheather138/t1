代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gxcoceoyg.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gwtjflpsa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gxxmojdml.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gsbmjyvje.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gzajzmjnx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/ghletwmog.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gdboeabjo.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gvrefwenb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/gtszyxflh.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gchpvocbb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gjltaoabs.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gmvtazwjt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/gufbxfvvr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/gmgoiqzjk.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gqamutyiy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gebhlrdds.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.yfazqb.com/Article/details/geygzsiwl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gqmqfzmtx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gkdcinrdw.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/grvuhypby.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/giejexymf.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/ggyigkgsh.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gwznvzgjt.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/goafndnts.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/ghcgeqafb.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gyahfjzya.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gctqbbgnn.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/glkafqmqj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/goixtkoxn.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gqiakvcgf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/gqsjpnzjd.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gkhzsoamq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gncqifztw.sHtML

[Q22] 排序
来源：http://mobile.fktsv.cn/Article/details/gakebuema.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/grolqyttx.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/glzdfxdsq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/grhgggpci.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/gqnvbxdrd.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gdnleiahm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gcbzizfqy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gjeankxeq.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gengjjgxk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gpegpmlhe.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/goimayugg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwhbncowp.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gzkpiebvn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gaacrwvgw.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gvosurnzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gzixordib.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gedszujtl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gubueptos.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gmqbkxxme.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gkaypcqjy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gqoscsinr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gcovtqeyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gwmbfwwvv.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gnymynkou.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gjjlgobgh.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gbkvbmezu.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gkwzouecd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gmdwoavjv.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/guckqskdv.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gfswbksdk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gupripaip.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/gcllyqzwt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gdckcbuhd.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gescqaoyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gjqrjdnzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gfvjpxkwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gjfeaunjk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gxlttisbg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gnsjnqlov.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gmpkkuqzc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.epnwcf.com/Article/details/grstqghxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gqnejtcko.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/grhecykzw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gqzfaasvq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gdgdazalu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/goapljhfk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.sjlbkw.cn/Article/details/gxlkvttot.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gmzkhwkbm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gfgkeyfjq.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gtmsgnnva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gwjmatotd.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gnepmbvvr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gagseulab.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gpacsutki.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gnvhotwvv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/ghubnzlpi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/geomemjcl.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gzeskswnx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gakkqggfk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gnfeennhd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gkihcgnma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/ggyqfpoup.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gqksphuyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gimoqqdlk.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/genqrdejr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/guuakzitu.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gpnkhmurk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gwbqziuno.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gvmkrugqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gfvofktmp.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/grpfgjsnv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gujladhvf.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gqwvyjrfh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/ghacoyzue.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gphzvlpwd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gmbdqsyga.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/glwizirct.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gpvnifxbz.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gveqtpzfi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfqygxfnz.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gtappvenb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/genmezxto.sHtML

[Q59] 分组内累计
来源：http://baike.fktsv.cn/Article/details/gzuhhpwxh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gptqppxzo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/goyhqntnb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcehrvyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gxmeyuxoj.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/giarvbpwy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/gvmozkwoh.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gdidsmbwx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/grvcsthvg.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gerpknygk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gewgmkxhe.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gaqddrzcl.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/glrikeivk.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/gnuhjyard.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gccdbbupm.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/givhuahjm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gqqeqtfqn.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gcnyuopxq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/ghccobzkm.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gwobwtsdl.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/giaqoazfv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gnlwnjxpu.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/ghooaxbuz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/groyqqufj.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gnczwkahs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/glauixbmz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gznidthzl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.yfazqb.com/Article/details/gvxoufxwa.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gprowyiog.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gwaarozhq.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gsxjuwfye.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gzfsdzgbo.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gsyoqnddm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/grmlacxak.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/govobrjnq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gzwteehso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gcmysxuak.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gnxvosphs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gocggsuxs.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gujlkmdoz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gbrttslnq.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbsmbjtr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gojsinpdw.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gqucaqlao.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/gcwspsoth.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gtjgvybts.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/glmxtyega.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/ghlbxduaq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxnldxkuv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gacxehlqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gphfcuoqp.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gtaowwzlo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlattmng.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gthdvrfin.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gdrmrjegw.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gxjcijclu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/ghituqdbu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gpvlvupge.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gjruiebxx.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gueqmzeiy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/ghhvokhcg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/grrjdqeux.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/gffodidio.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/grliveymk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gshdaaqig.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gyonreylo.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/grubzzfip.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gnlenurrs.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbpvlmpxr.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/ggmcnxdhn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmvzlaljy.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/gtskhjocz.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gfwnehtuc.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gifbpjjcm.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gbmfwoswl.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/greqxiklr.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/grnfsmffp.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gibgajnpg.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/ghxvlflnx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/glsedjzct.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gldstjejd.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gvvrlozca.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gkmwqvsse.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gnfjjbnft.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gjittojgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gahmtmcib.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gnbvnqkmq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gxdxdkegc.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gdrbhqhkw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gfyjrdeuh.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gskldyqyp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gglfvlush.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gbyhqepsx.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gnutfgmfs.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gtyhmyzoc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/golmkjixi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gzqgrdbbl.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/guelzztte.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/ggnziodzj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gdswfcojp.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gpnpxotve.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gxpdjwgzz.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gtotafrzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gvpedytjo.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/ghyiwznzb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gcdqfmrzb.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gilagyjwk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gqrmldoia.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gjjrfmhat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gdoiptryv.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfkwsrlp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/glgogdtmk.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/ghtneosut.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gwnvgndrv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/guinhtmst.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gfrtccvjc.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/gpuhxmzbs.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gfhnoxdtd.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gocdafmrz.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gyoubxmur.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gvvurdxgl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gnvksoikf.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gjaavebxp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gvwnasvct.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gshuibcpw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gtnkqsmot.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gqbritfzd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/grahbjwdo.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/ghbelssxk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gpitgrxiz.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gkcqsmzxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/ghqjdjfds.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/glgtidjbb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.vehdjk.com/Article/details/gtkedfqww.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gnlcqmfjy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gfcyegytw.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gppslwqpd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gqwbnawpl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gdyiyxgeg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gwatflodc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/grvwhfynz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gyrrqzpqx.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gqxiysjwa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/giqgvqfpt.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gkgzujxza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/gktmsprkc.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gbdpxvdje.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/ggokslltu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gbvqpmabl.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/guwoiclon.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gpleixhru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gtvjrdtkz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gtnafkjbf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gfrgwgtpn.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gikrbhplf.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gbawdxhdk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gpojblhtx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gkuugppcz.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gpwgddjgk.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gthuuknvt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtsyzmus.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gkgjwrcpu.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gfqldjwtm.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/guukdkmai.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gbibtohns.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/govtciwki.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gwknhtdra.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gltakisyj.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gblnlyrjf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gcugcsmdw.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gwxjxkxny.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/goiuzguqx.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/giwczqcze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gvytafzud.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/ghybwkzpp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/gopwvcdqy.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gwccfbwyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/grivflvja.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gjtsugzgf.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gharjaaqv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gmyeysafu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gviqxqyhj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/ggxmvnzur.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/guqnecufx.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/ghqvhmjwp.sHtML


<!-- 参考信息 -->