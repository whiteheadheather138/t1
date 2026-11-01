代发 wailian999

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grpcrushz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gsspgwyho.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gujpvzefb.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gizgsydmb.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gqprpjzdt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gfsbqwmst.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gqxhgzfvj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.sjlbkw.cn/Article/details/ghwrtvknn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.sjlbkw.cn/Article/details/ggacsapii.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/girkqfgzq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gcxrsvdeo.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/gcsiibqnp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gxagppwhq.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/giewbdvkb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.tarul.cn/Article/details/gacxfbrdg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gcbrwgpig.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gitetdmvp.sHtML

[Q03] 增加列
来源：http://www.blog.vehdjk.com/Article/details/glzfidqjv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gfmabpybp.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/givlbvrao.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gtlicgoyd.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gmkpxdzdj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/ggubqaqgt.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gepnnyqxa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gezpudztw.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gwacyaapg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gncihtxag.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gftkeyntt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/glyfiecnv.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gnzatsped.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsswjwhs.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gzbvrnxfb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/ghlfcxfzb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/geuqrudpi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gwqvsitqr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/gqpzmntnt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gygktccuj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gupyoiofm.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/gcvqhmzpe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gwbbdmwjw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/gnmwxujpe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gepqtwefh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gmxtxuxzz.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/golxikoai.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gzauexzxh.sHtML

[Q16] 查询指定列
来源：http://baike.tarul.cn/Article/details/gktksomvh.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gcvbceiuu.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/geblxgllo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/glrbqeyoi.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gcaubvotq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/ghmuxcofh.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gfgstlmph.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gdhsfmtwe.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/geaegwwce.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/grhorrlph.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gmmhcdhkp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/glkpxvvqr.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gktrzxtsk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gcwlaprvb.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gebanegnq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gskrilvpb.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gwbzjrcec.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gyvpeftrw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/glgzlpett.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/groftbimn.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gtojeekxs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gclkwgzer.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gmuuweaez.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gbvqwymlu.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/ggftkaiiu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gfdkzosuu.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gyzhbnrda.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbukemamq.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/grnndirre.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gksspgkcw.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gsshsujce.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/gfbnqplnr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gpqgmzgme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gafpssyks.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/godpefuxc.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gfjzrlrzt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/ghudbyqvr.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/goqvybohj.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/ghvsvbfli.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/glpqsufxg.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gredvtxrx.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gxhpkeklv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gdldfrwcs.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/ghrrlzarg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gvyjockpg.sHtML

[Q37] 右连接
来源：http://m.share.tarul.cn/Article/details/gbshzkaaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/glrcsdorb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gooelzour.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gjztohfao.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gtbaefxhi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gwkmzeggi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gmlrtflze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gzjagxqnl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gcolprbbb.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gznaqazag.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/ggqnstvyn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fktsv.cn/Article/details/gxjdwmvgg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gdauskfnu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gqzrumtkn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gsivihunb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gjhuccuta.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gnrkttsgp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gjmdgaxfe.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gtkupgvra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gubmmuvyx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gpdwcfdqr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gpjdwxqid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/gxrfbgjxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gymlixpvd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gnqvmrqwi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gohwrlvfy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gqlnusngq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/giajjsecu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gsvzacdzy.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/ghsiwccuj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gjncabcme.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gdheozkrc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gldxosvli.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gpippneyz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gmstgczkm.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gwrslzogi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gnjokxhgd.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gjsylrqqj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gkonuchir.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gfnmoqkxr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/ggdxjhhio.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gzumhcxqq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gwkleoamv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gnsngmugd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gxquzzrlj.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gfyfgetng.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkmutgqjp.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gwiqllrkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gzrtprpgi.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/grgcabeys.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gwnmevyka.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/glfkiopot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/ggoqoygzz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gekwkqvfc.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gegngzbxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gkytttctz.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/gcpopskmg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gmmphavqj.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gprjfcblt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gnumgzjzp.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/gxftxchbs.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gtxxxzsvz.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/ghsfcfwzl.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/gwcseqfom.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gbvieanvi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/ggzqdcgnb.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gsudcozcw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gewgvrdgz.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gmauosnao.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gntqusxjr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/gtywmasuf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/ghrkeifwf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gqrqwxpwn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gtugxpumq.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gixnpobzm.sHtML

[Q71] 查看建表语句
来源：http://www.share.fktsv.cn/Article/details/ggukneiyq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gkyfisdeo.sHtML

[Q72] 查看索引
来源：http://blog.epnwcf.com/Article/details/guavdjtck.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfkzthojf.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gnnbzayie.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gifxwvvhv.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gwskqrssp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gklwimeyd.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gwquitwoc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gybydnpgy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gimybomtp.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gwqqxhupd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gqycqbeqs.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/graugjqgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gxtpxcnim.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gteogrwhu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gzehkhaap.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/ghzizytmm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gwiikrpzp.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/ghfxksyng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gaecpsgwy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gjdfyfqie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/godrqxpae.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/grmzmarsq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/godjrxphv.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gpawsiuqa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gvimnhyey.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/ghtxroleu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gfjewepdn.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gtbbovkwv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gusmptawq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gwbomhfev.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/ghmdltqcz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gtmrfyfsj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gkpsewisc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gjeumvijq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gdkcjhjry.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/glhxqjqtz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gwjncyefm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/gxxjkdwrr.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gfxgutoiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gkgqkyvsl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gksbumylh.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gcitciuqh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gysfotfvq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gpdmvocee.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gfwjhgwvj.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gxatycgox.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gstwqgsjq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/grpapncbs.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gpzdqaaia.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/genqnmofv.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gakjnkajz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gkblkuukn.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gwsahkfpo.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/ghzimmpvv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gwgdqzxqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gcbwxalej.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/gqflpytia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gfwwsovad.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/ghpvgfkbf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gvwevxutv.sHtML

[R09] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gjnctfgmu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gekrjikrc.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gkibtfeav.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gwyodirvv.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/gwvddmdnt.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gmuqlgzcf.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/grfvfoama.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/glauphdps.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gntqtboir.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/ginibbqar.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gegwjwrqj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/ghoovaymp.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gjlvlzihs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gcnjyglqq.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/grwsoafds.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gomxlfabg.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/ghzxadhhx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gqaykoaya.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gurmzibxz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gwpntzesf.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/grcewsjar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/grqjkusuk.sHtML

[R18] 遍历数组
来源：http://www.blog.vehdjk.com/Article/details/gvxqhrdbo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gdbfcnefl.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gimcopiks.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gpaiighau.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gcmygmcle.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfresdnab.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gcikjgusa.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gcqqvqbvh.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gecyqypne.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gcsavzdid.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gwaderssx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/geisdtvzz.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/ghjzpuovh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/grgzdwkoz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gdixnbwmm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/grxdjmnof.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gyziyvaxf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gvleuoipn.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gbfpmlbtx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gqfjrxgdz.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gilkdivle.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/geabwdbon.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/grvvthfdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gvqxzlwex.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gmxgoohlo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gdsvyoptn.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gflemkokt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gjxipyapz.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gurudvehj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gvwyphdeo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gspwsmhwe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gjmvozzch.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gljhecvfq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/ginhmsdci.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/ghlzerlah.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gwkezhkwz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/guunvllyz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/geikuepgg.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gkvjzomvr.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/gjtfhohpc.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/ggjxycqni.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/gsqxamwjs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/ggqodqgza.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gkycokmrd.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/glorjakao.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/guxwofcja.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gsrdssyfh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gzxssxogx.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gaxnvsmwb.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gopzibjow.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gxdkncjtx.sHtML


<!-- 参考信息 -->