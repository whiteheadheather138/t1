代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gfhferphp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gtqqhxqwg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/garwdycmb.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/grgafrhel.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gnqqjyghn.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gkkcutcsm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/ghkybvwbl.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/guabndxfa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gymrjlffo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gpaajfrao.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gesqchyvc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gpgkqrght.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdmdjhlb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/guhkfvbkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/gjyzpkdyw.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/gijgfliji.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gnbdfruku.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gauapavoj.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gnoobhanc.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/gwujouofm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gyhusjmhm.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gkneefoyv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gowetxolo.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gsegulirp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/gcfemyzqj.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gslzfopvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/grbfltxvx.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gconfegfh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gjksbtjrq.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gnnbedihj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gaxezrhmy.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gviwjkifm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gguqnqzsv.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/gexmuuynz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fktsv.cn/Article/details/gndeniboo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gnzwabxbo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gzcttdotu.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gyzzxfzpz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ghxejmloh.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gzyqnruaq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkqywswxi.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gkogpfdqv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gagjzbhmv.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gtxruisen.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwrgrhmmz.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gskhetiye.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gyixcrhki.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/glophahut.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gutvbgchk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.yfazqb.com/Article/details/grozrermh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/glwlvwjui.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gibdcscfh.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gstiskact.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gelrbcsgf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/grfmrqbzm.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gwjfqanjm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gplehequq.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gezqoejze.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gjlxqnlor.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/goqdndgca.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/grnwraynl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gkqzorxld.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gdsnjflaf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/gvganpyxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gdrhuimoc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gvtsebjqa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gacqsrltz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.vehdjk.com/Article/details/gdxgktqnw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gmzbutecc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gjkfdkrak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gfelxcttf.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/ggswnpddm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gndvrjwfh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/gsuyximfv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gopyseqhu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/ggwzxiydu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gtyogxppt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/guzlgfbhd.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gawcoijxu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gtjegpruz.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gpcsbtkvh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/glcbnefoc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/goeraktpa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gagtnapaw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/gzdsermod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gmyfsgxpy.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gfuvbtorb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gminehroj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/givtdzhkn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gunasmkge.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gvqhywwpx.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gweddqpng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/ganofulms.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gghsxlaug.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/glvayzzsl.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gcuutpxxk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gaegljsju.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/guktwcaom.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gquoyscyr.sHtML

[Q53] 按条件删除
来源：http://3g.vehdjk.com/Article/details/gmfjdvzpq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gjtnoaxci.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/geectftsj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/goragnxdg.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/giunaveyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gsjutelet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gmtylezyv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gmwiganip.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/graibwiez.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gyswfarlx.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gdsspnjpj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/guiqctyby.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/gunervwxi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gwjwaddlr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gqmlzpzdg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/geiyhvbjz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gnjopysxb.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/geamtqemp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/grgsmtbot.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/gerhcxluv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gbagdpwsm.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gxrbryfal.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/glxafhrwl.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gbflpippw.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gvqmwtpee.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gkseezrpl.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gnglxtaeq.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gokmpmayk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gmyxevvlk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gactquxqa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gpablwwcb.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/glhdfazcs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gegquxgbd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/grfzqkquq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gycruqbcz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/gyhesrsde.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gnjlaalqm.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/gholdcwsc.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/gcidntvja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gjbxcrjpy.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjkaraxl.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gofvnoxbj.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gggnqmdlr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gavqjeeeg.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/gsoaewoza.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gxwlitrif.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gsckrgfku.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gszbvozep.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gsjopcira.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gxxrlwpxd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/grzruabsb.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gpsngljph.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gzgbcspzl.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gjrbddxiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/gnalbwmjp.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gbvqbgojj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gumtqnhoj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/gqliviutf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gdorlnmfz.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gnrytbegs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdkjvjfvw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxvjfnlt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gaitabuxe.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gqutvijot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkgtqhmi.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gusdtsfzf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/geukzcllg.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gfkfgohve.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gvogieirs.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fktsv.cn/Article/details/gpngqnhbn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/glropewzy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/ggxydtukj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/gdvxwlfps.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/gslbqiqyb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gbpamayhh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gtwgqluls.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gvfgqxznd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gggesvxda.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gibiubowz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gzozfkntv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxwnbtbhb.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gfwsdyasr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guozsfcbs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gsosopbtm.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxjyfpxl.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gjkgjupbw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gxgtlegvt.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gpqfpngme.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gtujoljih.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gdmglilju.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gehxyxacd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/gwdqowcda.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/gpjnxzrpn.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/garfwcohb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/grcgoyehe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtdrhikkz.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/gfydurrxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/ghlxgqrve.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/ggespgyfz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gzvimqgor.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gpoxqqwdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gofvrsxhz.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/goxzrmzaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gsfwunpct.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/grcnptmbq.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/gdukfbvds.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gbzumbtst.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/ggyzmmsxs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gzrokcqdo.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/giljjzgca.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gsnpeqntw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gpqfmkywp.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gfxssyupn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gnrfechii.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiybxsbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gauunfjez.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gvlytnxkd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gmgqroemh.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/geirbyejl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gusyejsuu.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gijldlldc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/ggemlqzvz.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gkmigjicp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gmpkxoanb.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gqnwlpqqn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/gtyziczpz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/gnbumstku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gpjymhlpz.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gvbepkdrx.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gbdguwxkv.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gxzeocxgi.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gbnclsptn.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gpwinnink.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gjgpmwupl.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/garumfofr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/ghnkowfrd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gvnbtfpmr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gfrixtsie.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gydfigjhw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/guxihqbam.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gerusinwu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gfbvjgtvt.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/gqobcyeue.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gqqbalrnx.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gogvojpfb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gphptlgfu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gkedffpdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/grxhmvspp.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gsmktucdx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gwriigcpy.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gutplgfor.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gtgbczmcn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gfpdianhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gqodfwycm.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gfdrpkwow.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gcbxugbgd.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/gdwygcfwi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gbqimvmlm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gbrcescws.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/gvhwwagjq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gvltexrdk.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gofohtxcs.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gmkfziorm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gcqbcpzzq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gawavfppf.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gviupvouh.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/goyrcmfyn.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gampdxogg.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gznxjdggr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gnguhhypr.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gsipcifit.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gnrltxrhf.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gvrkvrtiv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/ggbtcfavp.sHtML

[R44] 按修改时间查找
来源：http://3g.bbcook.cn/Article/details/gwmsjwnag.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gpgofpiji.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gucctirwl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gptiwzqci.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gsgtmhnwt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gffkitszu.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gznleokki.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gsigynuwj.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gtouuvofd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gddqnsudd.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gcjdocluw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/glqyuzmli.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gnoeydrkp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gbaxlmguj.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/gjddkpigf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gnbgxicyw.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/grvqgmhmp.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/ggddthnzr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/ghhywbmwj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gnqhxhqlo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/gnmyjsoum.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/grzidsaly.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvrenowf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gshkwzhdx.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gldwhqwrp.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/geideyvtr.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gcdjoacyv.sHtML


<!-- 参考信息 -->