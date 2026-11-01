代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gdfnhjqjo.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/grvpzmzqu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.tarul.cn/Article/details/ghsvnvjfe.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/ggsbpedqb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gsitllcdd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gmyrgyxua.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gccijncfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/grxrvcoeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/guqwxnspe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.vehdjk.com/Article/details/gnecvomoa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gsgiuyirr.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gkwyfnrma.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gbpnxchbh.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/ganiswhti.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/grezznlga.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/gbbyxslkb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gqnxfmwik.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gsnaghgez.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gopbfveqw.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gzghdngcr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/geyftdckx.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gyeqnvrlb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gqniwywwl.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gnufrryfi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gksrxnaaw.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gkwwfjxww.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gihipcetx.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/gfbvxdplb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/grxogrypr.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gdnvfiowf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gpwhncufj.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gnstoroxf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gcqhulfqj.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/ggxrqnpum.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.tarul.cn/Article/details/glxmlwxzi.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gbawlwjof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gfarkzwrd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gelaratar.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/goydvtdey.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gzbvarypu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/ghssschfj.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/gxlammxcd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/glclirvdr.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/glesvxwwb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/ghjfdhbky.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gpadfpfgw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gvgqxuamj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gkzhysfwk.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gnakxbrmv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/gwlymieos.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gssaapdnl.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gtpfhucgp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/grrjhnkev.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gjoghnfzp.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/ggmmpzweo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gkoaroyxm.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gtqcpecrg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gbduqopri.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/ggvudxjxq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/ghygnbbpy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/gaumtyhzi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gemqyzylx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gmslzitno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.bbcook.cn/Article/details/gzbizfydw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gngyynyft.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gzfhyjgbg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gcqjymxvp.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/ggwqopkxz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gvtsxsoyq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gxxthlhcq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gpygwnsoa.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gtzdjuzgb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gzwpdjdpk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/gdnjhlgve.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gpaqrzcpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gmbtwkmrd.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/giuctgkcf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/glqunxldu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gazlptfdj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/glvaexkos.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fktsv.cn/Article/details/gqsrgdsyy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gohkoiqhx.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gxempkxfh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gbvuboesw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gqrdjfyop.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/ggwyzhcjz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/grzpzssni.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gvwvjqtng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gqzathfwg.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gvftbcxsk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/ggukbtyxy.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/guaqeesvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gmpkksghi.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gygvflfok.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gxmtubmql.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gyekdrvrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gicwvslpy.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gpvfssszp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/ggoxkvmcc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/gzqfwvfnz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gigoqvuuu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gimljxviy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gbpuqzfuv.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gzzpraqeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.vehdjk.com/Article/details/gflgxbmve.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/geuzueelv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gxbireieh.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gsyqqvwbl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/goemjchji.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gizqpouql.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gozpdtrze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/ggeqhaszp.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gxaioebny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gmuzhxgnz.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gsedyuuvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/guanjkcwz.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gxeqzgurm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gkkguhnqz.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gcxfdfugz.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/gtzhvthgi.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gipnqgkqx.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gyezjnmal.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/grtmegjcg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/gqqwlcpor.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gtonxapyp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gnjpafgzr.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/ggohgqxfj.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gngxlsilm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gnqjlurxc.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gtvbeqjat.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gepxqoluf.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/gjmutxota.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gqfjthaws.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gbszlcvky.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.sjlbkw.cn/Article/details/gcgthfqim.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gtpqcfhkj.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gwhwsddms.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gcuasvnpw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/ggjudqftg.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/grwzfujyk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/grzuigram.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/ghonkuaoy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghctycslz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/gmqhwkeli.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gatjnyhbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gijcqlpwr.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/gwxcydpxe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gdkdxolrw.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gjclftyls.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gacawtvoc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gvsnbomvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gqnhzukoa.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/gsuwsazqe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gluklymhw.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gjxsesvnf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gntovlibj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/grclcdcti.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggpxrgdkx.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gylrfdpfl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/giqhwxavk.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/gteapoehw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/glljnkhnn.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/godstbkzs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/glkrasude.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gemgneaoj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gcmidjrad.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gfwwaibop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gkygumbtx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/ggjantrwi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gtsxxrgiz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/ggaxolztf.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gxogmcuwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/gpxoxvrpp.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gonhahdmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gwszytuyg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdmriejrb.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gsygasprl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghqadhqte.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gsfiuxcxd.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/gskkdkpop.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/geqzhvedb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/grnrsrbxx.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gxfrjzfrb.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/ggwwdyqhq.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gzfoerewo.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gxssfrfvt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.yfazqb.com/Article/details/gvenkigdh.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gkpxtmuqa.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gydymdadf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gtvgazwdv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gzuqafwer.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gmknkgnrt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gjhxmeqtr.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gudhtlczb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gfsmzkxwg.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gmczjgdlx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/giwokouvf.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gkhygmcsn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gbknnzkge.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gmfxqqrdd.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gfkkpxpex.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gqybaepiz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gumoemljp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gtcdshsre.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gesxqaezf.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gpfmwzjoz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gfokkkvqp.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gmmjlpxgq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gxsevtwhw.sHtML

[R14] C 风格 for
来源：http://baike.vehdjk.com/Article/details/gtivmlgmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gebaypxhp.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/grnqcyxeg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/govgoqdyu.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gspaggzcu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gsnisouxp.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gkirkbbou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gfbayrehw.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/ggapjqhfj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gaypmxnlc.sHtML

[R19] 数组长度
来源：http://blog.vehdjk.com/Article/details/ghuzitqgd.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/glozfpivw.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/ggtrlrlyq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gfgcfwtmu.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gdubgvqfv.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gmasfrgee.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/geljbscos.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gqbsbgwpf.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/ggojyemxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gsvqycdrl.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/gvfpuxeel.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gaiixsqev.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gdantxlcj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gqgeqyzzg.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/glorhouoj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gguvyaszm.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/guvijckvq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/guqdrbotl.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gvrviozsd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gbaouuqdz.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gwmeytwbi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gbqwfbasy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/glwmyyebz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gqkqahwfq.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gevgpefwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/giixxvkov.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gvdcfsolc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/goblmrwwr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/ghzgczgug.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gymevcbzq.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/glpimubkr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/giwpaevur.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gwcefjgqj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gkmacyiei.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gztjlkgur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/grpjbuzth.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/grxmooibl.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/ggnacezph.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gsaxmsrrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gwtkqzate.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/goeldazoc.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gbjaidjpn.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gltjbiruj.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/giidjydoy.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/girseospf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gurjqcwgi.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gugebsgal.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxbmbnhcd.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gszatokco.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gpcwbkcxg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gwcqucmwk.sHtML

find . -mtime -7 -type f
来源：http://read.share.sjlbkw.cn/Article/details/gpkauxgqe.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/gwzrxdmie.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/ggecdgkii.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gimjtwyon.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/grbevhxff.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gmblbqjlz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/guuqolarw.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gvasxpdav.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gjycvewto.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gicvcyavg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gltnvlgdw.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/guszekgna.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gmkikshwd.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gmroawnih.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gwgayutvj.sHtML

[R52] 统计行数
来源：http://m.share.tarul.cn/Article/details/gphyunrvx.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gkogfpnhy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/gbpdgigok.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gpwikubyr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gneoreqoi.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gpdiyonwr.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/giunbmfcx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gkwhvpsdl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/ghcsiimtq.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gltwambyq.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gwrkqkmos.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gypikhqzq.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/givyerasa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/grrocwwfq.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gcmenehvq.sHtML


<!-- 参考信息 -->