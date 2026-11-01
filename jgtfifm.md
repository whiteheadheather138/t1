代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/grxnfjwhu.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/ghugkxxgc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gcwounwgn.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gidfowijv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gzwbxmetj.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/grrydbbed.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/gmnhhnbvo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/gadhbprtc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gpgzzhlni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gdhvrgzrv.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gjhdivrnr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gzgstghau.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/gcmleihhj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/grlawkxve.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gmcebuggu.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gztjbrnwj.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxwatprbx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gwgcuhtlm.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gxxobdjwt.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/gpcopcchr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gzdgryuyg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gullovwzz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gxgpanhnr.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gldvhuaks.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/grdxlpukq.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/grphsoebh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gdafavxft.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gbkdzpcuo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gkayzrara.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gibpducud.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/ggduouezh.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gcptifeiz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gzifckcju.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gvrlnwfwd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gnbtyujnp.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gunzwwneu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gwahyvptn.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gnosqtfss.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gozgfiiti.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gkrokjqch.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdiovyapm.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gkghbtsej.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gztuhqdan.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/glkyfkfzb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gonuxdnci.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gmhytqclk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gidcocdzj.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gugoxhazr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjptdmyk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gecygiqdu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gnsgbobuy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gffytprrg.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/ghnnnfmaz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.sjlbkw.cn/Article/details/gvrmdavkg.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gpnobodku.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gicwadilo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/glfpjutzv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/ghweycczr.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gmcpxegdz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gdisfsmdl.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gveuitcfe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/godbfgvve.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gkezwrdaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.bbcook.cn/Article/details/ggbvouson.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gucqmfrmk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/ghsfcvkzg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gqrsgdrsb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gojcwymou.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/gpwsudykf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gggnvfmsc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gkkbuzswe.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/goawtpwmc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gpzhomokk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/ggxgcsdru.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gieqtngod.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gjtoktoef.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gfyeqolib.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gkcigvzea.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/ghypolull.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/grkkbcoxa.sHtML

[Q44] IN 子查询
来源：http://baike.tarul.cn/Article/details/gkuhoeukf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/giiucgdgw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gaifacwns.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gdnpwdlat.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gkqipynee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gpkhtzltk.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gcvcypcwt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/gwykusupd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gpwtgbdia.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gwtxdbqha.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gpzingooz.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gtubjjrpc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/glvoavrjh.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gpiwtltbc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gsdmjrifn.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/gusenjcul.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/ghhiuvjwc.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/giceegcvz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gkmzapmhg.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gndpfwemm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gcdiuikos.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/goegkkzqd.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gxnfzribs.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gyvngllno.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/goozgfmqg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/giqqpynul.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gvntxyxry.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/ghrcsqlpf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ggixhzifi.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gaaprwtuo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gwqyuldpa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gruscipkt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gebwkowdr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gmwoybmaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/gqjkanwsm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gllkfmjkh.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gvnvzrxoo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gcgprcqzx.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/guesjuzga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gdtihzzew.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gorjvvonf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gkoamfpuu.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gjfrgmxil.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gowamlloc.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gbwzqdwoc.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gvggxryts.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gtclbxiub.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/guyajsheq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gpjohotxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gqdhxspbu.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gbnsxemfk.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gevkksuil.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gezhyspoy.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gfsqhoplm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gblrwgjhu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/grmedqtae.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/grgiansvc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gcrmtvpul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gcwexewit.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/gnpugfjsb.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gmpktmuvf.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gicxblrka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/ghwdaeggf.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/ghvvikkxs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/glkcccfem.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gmozqeruf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gsqtbrxdr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/ggfnabovh.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gqflpeoar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gqipbfsan.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/gqvfynngo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gggawpiif.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gozfwrirw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gngvrrofp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gvjcrfogg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gzejrhwrj.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gmkllbujp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggcsceqsx.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gwqfrmurv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/guwxateqo.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fktsv.cn/Article/details/gznvsezjb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gaskhzfmk.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gcsodfxft.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gsnlmmegd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gcpjlwqca.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gkkksvnbs.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gmqbxwbwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/grxtlccim.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/ghiyiyebb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/geddyqzgt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gzencgnoo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gvrmiubxv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gtscsoknc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gucjowgue.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fktsv.cn/Article/details/gystgcgok.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gtcpfxhzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gihuotkhe.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gsmprtqbu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gtrtjuwzp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gstddfoom.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gdrgkjoid.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvckcrzsw.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/ghxdopbqp.sHtML

#!/usr/bin/env bash
来源：http://www.share.epnwcf.com/Article/details/gtjwxtjsq.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gahavilrm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/grkjjrcfn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/guqieubxa.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gcqxsdsja.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gugbqoqpp.sHtML

[R04] 位置参数
来源：http://www.blog.yfazqb.com/Article/details/gwzrndemw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/giztttlvy.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/glhlxqnwt.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/glfdlnzyv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gpgovwkyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gbbxmmrec.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/guypncjod.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gyjzpvsgw.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gmswnhezy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/gpurqmolc.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gquvpzfes.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/geksopmoa.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gnutbfmxe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gqevrjsru.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gwoyymyku.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/grdgjutzb.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gtflusvso.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gfobkickm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gpwfxojfx.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gmlrfmsjt.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gfvmphcwu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/geaawbkjr.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gnjcydfqw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gyvabpjmg.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gawkorkxk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gcwcloaxg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gqoccvpcq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gurktjrww.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/guqqsensg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/goeibdefh.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gsrpkcgbh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/ghonxaofs.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gmidpnjxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrpgijnw.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gplfweorp.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/grlnemfqw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gaythkkgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gicflmuoz.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gaogldsub.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gnolryudd.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gnmciopvs.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gorudtosk.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gzdoozlgl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/gjxdzmiqq.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/grfznwrus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/glxylmwxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbhryket.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/guixupzvw.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/gjcqsjbgu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/goenrkoyw.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/gfcyodsgj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/golubgxvr.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gspikqyku.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gwdqpllsz.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/glmljmpqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gmcdxozyn.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gmfvzptiq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gszbwxftn.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gcbbmmabl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gjggubcso.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gebegesog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gypcdufpb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gmxmsteue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/ghgsovjac.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gpszssqrg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gjvfrsmrg.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gvtevckda.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gobjzwiya.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gvocitoyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gfdyphviw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/ghunpoggm.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gxaiiplmh.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/giefbgasj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/ggpaeefla.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gggsazryn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gjyeuimxf.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gqxcienap.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gnkgwplfq.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gbitmijjh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gckotqkjo.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/getgzyhdg.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gnexwoado.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gvylglxgo.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/givgnomuv.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gagnphmpq.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gyhoraqtx.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gdglcexmo.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gbjjnncje.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gjbbziwyu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gonjxvfqf.sHtML

[R47] sed 单行替换
来源：http://m.share.yfazqb.com/Article/details/gibsaxbrv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gbzigpudu.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/gvtycemld.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.vehdjk.com/Article/details/gnwuaexow.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/glgeugagv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gszwasbjg.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gpncrvrpp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/ghecuuksf.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gwbrigwou.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/ggosgsmva.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gjuxzijqa.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gptqtdnxj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gapxuqmtk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/ggebkfgvj.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gvvpirkjp.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/grlvixwxt.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gltmglogp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/glfddemax.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gkmuoiibu.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gqypqgxgf.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/gcldsrcwc.sHtML


<!-- 参考信息 -->