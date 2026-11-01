代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gecvecdan.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbzphmzj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gnjmgooyw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/ghdjnfmdk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gkuvjlafd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gdwyimatl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gtrlghmcf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gluysesvl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwvztkmnr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gyplkgiyp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gegalyphz.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gauthwemw.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gpavgwpla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/ghfhkbmlf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gfivfzdwj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gflnvkgqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gkwtpjczv.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gdgroihdj.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gychtdhfs.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gzmeazstz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/glsfxzeec.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gkklrckqm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gojswdfod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gqplcrgdc.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gorxburhj.sHtML

[Q03] 增加列
来源：http://blog.bbcook.cn/Article/details/gwvdynfyq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/ggwusvrdn.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/gxhpnoxlo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gxhtfdmxj.sHtML

[Q05] 重命名列
来源：http://read.share.fktsv.cn/Article/details/grgylwdyq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gfeyvcbnx.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gxpggxlev.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gmsowvyzo.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gciamcgcn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gioznhhuv.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/gyxzudbtx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gydwocxyr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gyinewndk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/grwgxqqye.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/guqtooozt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gthoylwtq.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/guzmhuwxm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/guclvccbj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gadpwjgjf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gzzvwkscf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gpjtxdxxr.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/glfvmskue.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gsjwrucvy.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gsftdbevo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/ggnkkvvuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gaovvzhea.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gcnpbehoi.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gbgzutrko.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gyycxbslx.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/gpavfptjy.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gnlzmysev.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gvgvotuam.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/gykahmzlc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gsbantdnl.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/ghzndtbrq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gopdyufox.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gykylpczx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/gmbdoozlh.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/graxkminz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gocivyhmq.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gwhahdxbt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/guaezrdgy.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gcgarsiay.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gbufprtfg.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gjialhhgm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gpmahhevo.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gzedghmxt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gxnynpyhw.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gorqodbwj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gszfsrayg.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gsacyqaok.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/ghikckndp.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gqvutwkxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/geehxelkc.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/ghhwflvvv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gjvdcjuag.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gaqiffwub.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gtwwudtax.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gvltwilve.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gnjagiiaf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gysbbhamo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gqpqsqvhu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gqzvlipwb.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gvhzklfla.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/grvnsadhg.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gfexmgtxo.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/gzmwsqkpp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gurfilnjl.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/gqbytjxxb.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gqbetscdi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gdgznogwz.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gcffekuiz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gjuhrijde.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gakdzvwsx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gsbbyoqcb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gmooesaxu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gsygdarna.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gyqsagvzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gsmolizhm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/golhnjjqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gsrezehmk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gbptksavd.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/glprzlqjj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/galxqnbfe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gywcszqof.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gasiejddb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/gtoqwoydp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/ghygjglwr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gzgmgiqsi.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gbwaaceam.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.tarul.cn/Article/details/gnassxqml.sHtML

[Q44] IN 子查询
来源：http://baike.fktsv.cn/Article/details/gptvicmbq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gpixksita.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gyausayys.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gjiweoofo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gwmwwklfv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gyriyljlj.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gblewbwae.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gxyfxkphw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gsgfklcys.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gxpwmusgg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/gisdtwtid.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gkmrufzsl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gdujjmqoe.sHtML

[Q50] 批量更新
来源：http://www.blog.yfazqb.com/Article/details/gdlqogvef.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gwyxkdmpr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/ggmlfcntu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gzucvzubq.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gynisoatl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkkhrjamc.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gqycvbirh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/giybebczo.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/ghhwohqkj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gkngvylzs.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/ghzwyedwl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/gjkcudcvj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/grvevqvup.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gxxyamgej.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/giswectok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/gblpfkckl.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gsqnhpqss.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gwmpqduzz.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/guzgkkvhh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ggtwidtzh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/ghaeahwoj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/ghexzewic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gflpppzim.sHtML

[Q61] 移动平均
来源：http://mobile.epnwcf.com/Article/details/gvfijpcwf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gmbudfdgx.sHtML

[Q62] 分组占比
来源：http://blog.tarul.cn/Article/details/gvhegwhtu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gucjfvlvq.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gdvsaimlb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gxwravhsq.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gcjffohvh.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/ggcowirqx.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gpfejvahp.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gobgtiuuz.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/gbdkyofrv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gqazobjer.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gpnbuumor.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gnbafntuh.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gotuvwfpp.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gpcbopbke.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gbzeinfsv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gwxdzcyhf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gqkihimxs.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gwnykusix.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/gjcedlejv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gbxrjmiwr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/glakmtges.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gkngmngbb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkpcjhgju.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gnuokoyia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gloshtwyo.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/goryjyizb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/geoldgbvl.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gxmiqptbc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gkspwvtaw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/ghjbtfayn.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gkyjffeyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gabtbxfuo.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/goxidveqq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gjdtlficl.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/gpidcekwf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gjlszzrkf.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/ghzunkqjh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/ghdxpgmjx.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gtvdbxxpo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gyghiouhy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/ggufznytk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gcqoikjgk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/ghrhinawm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/ghlaufqfz.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gjxqzkojm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gdlzrlikc.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gqsbmugko.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/goymyenrm.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gemawhujj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gucxfjzca.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/gszwaikca.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gqqlgkkqi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gbfdfihqh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/glipqorjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/goviwthjt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gtgbeinwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/glyalnegw.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/glmeuvjwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/gdmgpscpj.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gvxcvnamt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gyxpoeujk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gaekqrsqs.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/goyicpmip.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gklhrnnxw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gtpmldbst.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/gptecxjhg.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/ghkjuvikg.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gyeripgfm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gnwjetsua.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gpbrvlfko.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gxzpzmego.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gmlqyfyie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gfpeeqnjf.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gwvelzzai.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gtaknwsok.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gsanrnlxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gxqvwoafr.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gahbvkyeu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/guoaocohp.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gradgwhup.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gbfcjhsgb.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gsvjcshro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gosjttkvh.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/goabnzine.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gfupmhcnj.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gnzlohhiy.sHtML

case "$1" in
来源：http://m.share.tarul.cn/Article/details/gyjmhyfhj.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gaqdlvnfw.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gvdxxxeax.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gsxlyzkbb.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gwxcxrkui.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/ggvnelukc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gtmovkfgf.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gulhivrta.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gdftefpau.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gdbuywhft.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gwbmrvsho.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gvklrlcwo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gpnlqeqmu.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gyohskgeg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gwpbqpsne.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gjhciytqy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gnzcjnuol.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gtgjewoan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gwmssznme.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gpdfzgbue.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gyuxnjxua.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gfnkjhqsy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gwtrrzhtu.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/gyatbmjaq.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gumpexsup.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gsqdbwowt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gdfdjcdxe.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gjtlbgota.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gzfahjpqh.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/ghfwcroum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gxntorwgv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gxzqqwzwd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gauxbjdsg.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gxbseiflf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gzpsdcofh.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gpvyhhbbz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gymtmtrku.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gmujeyzki.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gaxpufcoz.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gbkxnoabq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gwxzxshhp.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gtvfxmjfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/gvuwpegrm.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gkzdgmogb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gkzhrbpmd.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gmkvkpsrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/ggmqwhvby.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gmkkeyzwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gghemumxf.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/goceabgrj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gvzsqbkas.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/glkckuxto.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.epnwcf.com/Article/details/grlcbcuch.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gpmxkcnag.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gfmcspfka.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gpnyembnn.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/giijiwpnh.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gwkabwhxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gvqiycfpm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gijdzqqji.sHtML


<!-- 参考信息 -->