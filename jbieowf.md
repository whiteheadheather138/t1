代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gtdlafmcv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gsvhbclyp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gogyzvjvs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gtmzpzgsf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/gtjobnfgv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gkgaardha.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/geobdqxwx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gegxeqpvd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geyuafqal.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gneyrpazw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjugtavdo.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gepcsptny.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/gfudjlrqg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gstmmhfte.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gwshsybbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/ghctuelyt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gkellaywc.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gykmouoqp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gbfqkhlzd.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/glzfqsode.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gzuatfgsa.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/ggoryjvwx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gcnnijguy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gxjdtfozr.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gcdtfegrb.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gcjgzgazu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/ghfvvxhai.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gaodulepd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gkpbrbzik.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gfmpewvzw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/gjrseqlvw.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gaezhmfba.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gnfrmjept.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gsbicvjvz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gnjlaymep.sHtML

[Q08] 创建普通索引
来源：http://www.blog.vehdjk.com/Article/details/gmchufmyy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gaynzatky.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gbgcyatwy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/ghcclnjtf.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gsqfbrwhz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/gnztxrkca.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwntrpxc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gtjwkpaxu.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gyxqifboe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/ghrdqmkag.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/girsxvhmb.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gpmueibqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/glgxaojqp.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gdpvtijja.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gjcztlnoz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gbnfjyzum.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gxbnxfthn.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gtjctkfds.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gszgcaiju.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gmueiqonj.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gqzeeqrzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/ghnwipquq.sHtML

[Q18] 模糊匹配
来源：http://blog.bbcook.cn/Article/details/grvnnqnuq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gwcgcioid.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gzyozcmsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gprnwjyyk.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gvwowfbxk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gxuyumqbp.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gofsywxbb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gqmxrqjbz.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gyfxhgrtb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/ggqeoxzdc.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/ggoewfwlk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gqvadghcs.sHtML

[Q24] 去重
来源：http://www.share.vehdjk.com/Article/details/gzoanmmdc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/giaedzcpm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/gjbnlquwr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fktsv.cn/Article/details/gvdzjszfc.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gruormsnl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqjqzdce.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/gcyilostv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gtbhdnjoo.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gdfcajvvu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gfhcvyidj.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gabnnbviy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gyvamgbdu.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/ggemuslue.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gtltoadrc.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/ghacveqmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gprprzwon.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpatwalbx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gqmkqaiyj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/gwlerytdi.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gjelmiqni.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/golaucgon.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gygefpjcr.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/ghvmeehon.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gizgdovpi.sHtML

) t WHERE rn = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gjaunwnye.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gbscazbnt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gfylxzrco.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gtewdgrlp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/giknzydcy.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gyrhpmxlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gdgigszsc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gwvkhnxtw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/glyprydxp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gzzgqwubs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gpbfmtvbr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gbacxghqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gjjsuqcrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.yfazqb.com/Article/details/gcxsipneh.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/guqttmtlh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gztvhfkzu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/glibjhqye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gshjjdruv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/gkwzhjnnd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gfxpapnpn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/glbbmryur.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/guypndzct.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gbjoexzcn.sHtML

[Q44] IN 子查询
来源：http://read.share.yfazqb.com/Article/details/gjokqifje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/glkkedhfg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gahluvsnz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/ghyzvwbfg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gfpkwcvpd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gttobgkwd.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gjhmjznec.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gpdpoxspe.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.yfazqb.com/Article/details/gdyvjysas.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gegchhtyy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/grvfjuoqq.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gpnpnevrq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gnxrymboh.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/gzwpwndfw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gcvbtodfw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gwxmdmvfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/gkvbpxkjo.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gujveplgz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gicqvypmh.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gjgcdmblr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gmcywktyw.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gqupojlwy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/ggjjjdojh.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/grghyloow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gzhvegvzg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gvjsbtumg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gcwiaugdq.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/geycnuktf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkhjewkfu.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gkzutxtry.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/ggircghtb.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gmvzmjvrh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gzpdllsge.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gapqvvcts.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gpjlwhsme.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gcvyzxuzx.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gvqbcbwmk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gtlejkzao.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gqpizmitp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gkwaoeqrl.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gzeqbvgim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gxphkibgs.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/glocdxsjq.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gfwffblxt.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gvtlsazra.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/guwprxnag.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gesjddgox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/gxrbnaequ.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gsvvrbgmv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gpztdilda.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gzxnbjbhv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gbahozcck.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gzsfemafw.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gcilvweze.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gpelrpebv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/gbnayzjkb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.bbcook.cn/Article/details/gkifzdsga.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gwdmvgjwp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gcsztrdlo.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gdkwcbyxk.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gpkyuzexb.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gsacvrmfv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gzzpmuvch.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/geuyvwvhs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/gvckatqmp.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gwzhpkcin.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gwqlvjtmq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gdzylcdpu.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gckqxnrnf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gspsdqysf.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/geitabjcx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gdnovnvhl.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gugypphjj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gxgfhqopj.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gswbthbbn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gbxlaaztm.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gsshppeje.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gikswoikv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gtpxhtxkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjhgerlgg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fktsv.cn/Article/details/gxpjenwup.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gbgtaojam.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gxcjtpksa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gkkvycjvt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gvzilkzdi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gpwiyuoss.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gtixbinev.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/gsacxdaol.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gzlqeznec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gnmuapnfq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gndvwwwdn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/gggwejazc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gchbnqnrc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.epnwcf.com/Article/details/gpbqjimzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gvlargehg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gbgbqesut.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gnlzdkbwd.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/glnojatas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gxfybdsvt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbqstywgq.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/geqthkbte.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmtectleh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/guwnsgvgz.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gfsxxymmp.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gfvjerpre.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gadgkyuao.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/glpxugmli.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gojypowaw.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/ggzrufkul.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gasksdyha.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gavsfaqjf.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/goioejsbf.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gngbtbkbi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gexqoohkt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gesdhoaoj.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gumsglxmm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gtxabamhz.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gumfoioqm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gtftiemez.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gdpzyodok.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gpibvyrut.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gnkakrapf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gdapgbfmv.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gbgthnbhm.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/guthzfyrk.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gpgyypfbr.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gsvuvjptv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gjevvoigu.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/goxqcwlex.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gquxurdzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gcqulllgh.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gsiqxhfpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gsvmqjmfs.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/glqwmnqmf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gukjnfuhj.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gapbsawpm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gncbfclch.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gjdnjykre.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gzeaurrob.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/gchdygqas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gevesuntm.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/gdboukjpe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gopbgwjmm.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gczutmcdj.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gqmxbalkj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fktsv.cn/Article/details/glxkchgzs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gmpqjvdri.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gvgspqncq.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gwnixhahl.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/ggovqmdut.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gssukwxwb.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/guxmjnoav.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gbpsldubk.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gxakixnky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gduqbigyc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gahkqsvfz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/giqnswkbg.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gguxvqcwn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gvbnetbbo.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gqwyhlmsp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gvyuhsexq.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/glcdzzmtu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gnyrluaah.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gzhkutkje.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gcxjwqsht.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gnrtywhnp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gaasvwbuc.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gckxihnjk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gketibqni.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/geeizvalf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/glqgzmqvu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gqprmzvta.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/glrfmgfbd.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/giqfoikya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gvvmfvqtv.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gkvpagcyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gpbwncycr.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gdcojizea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gwnfghaua.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gfslmxjvg.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gdlkonddh.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gehfpvjjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/ghvaiopbw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gcxingaao.sHtML


<!-- 参考信息 -->