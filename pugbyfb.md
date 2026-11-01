代发 wailian999

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gspwkpjms.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gmidpcgvk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gbbwesxwk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gvftqtudx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gjgibxxlp.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gofisyulb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/ghunwfeje.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/govqpvujh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gimepttpe.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gamepdzjf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gffwbuweg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gurjicyex.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gxwcyiitx.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gjtmtgbrw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gdwjdjdzo.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/goxjqdsoa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/gphpgwkod.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gwgmsnosa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gqrdnwjpn.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gtupnnkpk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gzvzykowl.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gavbqyqwe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gwcnmoilb.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gxkmomjup.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gqcjyqocu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gysmooadw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gysmwfoor.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/ghmlpgwog.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gdgyiigac.sHtML

[Q11] 一次插入多行
来源：http://3g.vehdjk.com/Article/details/glmrprsfh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gdxjcemvu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gcypxrdhs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/ghvxagqfi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gnhvlyrkc.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gmmkwworq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/guaeaoods.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gzirlwclr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gvkumbghi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gicyqdemg.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gslckkdbx.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfrizkmgd.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gukzflkvu.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbogifdjv.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/grbqhltvh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gcnoxxpii.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gqmwvqvoz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gskmiaueg.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gzfrmjyzs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gsmfbiqpp.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gcocbceqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gbscyfoku.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gtboomclf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gwmvepuyg.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/glmcwluxy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gvmtprmyt.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gpsnzhjmw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gwebhfewy.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gdyvwwwwt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/gjxmphozy.sHtML

[Q25] 只取前 N 条
来源：http://blog.bbcook.cn/Article/details/gvkwgeggj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/geibmmdul.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gfbpurjou.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/guxafocoa.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gaktrwjti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gfuuywjof.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/guotvsmig.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gjuhlewxg.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gwoipkzhx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/grkknuqhv.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gdavdltrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gwkzsbjws.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gvuusvxgd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gehlnbotr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gcfqzfsxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gvbzmjvnv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gtsnlaxla.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gmoalfnuz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gjvnwhypv.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gqrfnlxyh.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gvfjnbjxr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gpffdsfvn.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gdaqlnsar.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gvsmpqrlk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/grzcygwei.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gzhlzahxo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gkkshrmjd.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/gpytusrps.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/ggzgopext.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gehbbsxnj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gnpcqnfqi.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gxrerccmg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gucjybekg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.tarul.cn/Article/details/glvyhxnlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/ggogykgsm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gjdlrnyrg.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gzvmiboiq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gyfxdiuyk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gfnmdnxok.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gbmkjdujp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gbhoptsgo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/gnqldpdjf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gzlinbfil.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gpngxitlf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gesktjdjr.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gvridteng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gfzcnbwzk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gplzspzdc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/glcogxugs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/gidobuntm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gajsbontu.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/gqhuzsjox.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/grbvxersc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gmfrmazqq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gsjmikvtj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gyjlkqwrd.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gpcpjzyxo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gyzksxjdj.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gjcivyivd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gvahagghl.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gseoqycdv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gcycmgwui.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gxcqzpkym.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gnyesgibz.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/guotjjmpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/gsgnknqkv.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gdjwtgkji.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/groxasssi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/ghqzsjqjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/giopuwnku.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gwpfidfoq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/ggpaubsry.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gaxblujgm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gbodjeggl.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gzjzywebc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/gfmsxcglu.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gpaqqgrno.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gilyvrqcl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/gpgoscvvd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gxscyqwxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/geapvacrz.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/grngeygeq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gqawnkbxi.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gzpdoqobl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gyjyobzrb.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gcbdbpvan.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gbbabnfhn.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gvxpybaww.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gnqlvnhex.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gvpptxwja.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/ghrepnope.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gvpvyizzn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gubxlrltx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gsoowtqdi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gfqfwbjlu.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/ggkumfvow.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gogqshrmy.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/guvfjeopd.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gaduqazwq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gqltrskfi.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gurrzklwy.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/ggntritwv.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gbujpijtz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/ginqqifcd.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gutvuayyu.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gcmukcryr.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gmverbevg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/grnuhsdaq.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/grmevrowx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.sjlbkw.cn/Article/details/gqhsfbkwq.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gpqrgtztw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gfkdqiecc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/grozltjic.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gjpyemnvx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gfqptfrvy.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gkbvfjgaz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/gjuvvomob.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gvwmtulvl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gufegozux.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/geqduplzh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gljbuochy.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gfpaevpaf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gcjqyklma.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gppzatcoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gvjxfbfxm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/goqkooskp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggiyhfkfq.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gawmlvaxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gemeilvqf.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gsrcikwgk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gtroperdw.sHtML

[Q85] 数值取整
来源：http://read.share.vehdjk.com/Article/details/gtshrmgyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gaycghqba.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gequedsyg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.vehdjk.com/Article/details/gczuitjdj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gkcieeqsf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gmzzhdiru.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.bbcook.cn/Article/details/gthdtxyzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gevnbhfoi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gthlkhokc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gnnhjfwtn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/grjoujrwy.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gmzobnuwy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gwhqxsymv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpfvunszk.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/giygtkzzb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gycfplkhf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gnaoasbow.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbkknvcx.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gpgfazogv.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gxlwsfyhk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gezqzciai.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/ghznviblr.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gthrkewcv.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gvphgfvxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/ggdreherq.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gnzdoepwf.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/ghokxwtvt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/gwmrgpipv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gvgqjoqxb.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gnlnpwxhn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gefdkyjft.sHtML

[R08] 数值比较
来源：http://www.m.share.vehdjk.com/Article/details/ggotauxss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gzxxtpokp.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gthithtzk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gttpcuxwd.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gwxotjaqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/ghsgxvdwe.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gfxbqzkwx.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/ganlqizdl.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gmwcdcitn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/geflikwyl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gwasnhtje.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gcdnuwqfe.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gndnvpkvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gmoecrqen.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gzggpwhdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gewxccxjc.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gtaclbqbg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/ginpbwdpr.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gyuvomwdu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gechskitt.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/guavymwll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gcisqpnez.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gekljmhrm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/gzxbxwyuz.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gefvmsttg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gjzqiiumv.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gyxmshkzh.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gymotheub.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gdybvcrgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gizdiultz.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gexqxomcl.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gtpqkzszg.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/ggpihbzks.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gjtcfiwve.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gvsdemqjy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gupezxkil.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gdcmumdvu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gdmyrnapp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/grgksuoxi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gniibvruk.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gudvampby.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/ghscicgur.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gjqjeegua.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gzsdoqiqc.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gbeqhefnc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/gmaqodivx.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/guxmztden.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gwnbuykdr.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gocbmirie.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gnupjamku.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gwkftmuwn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gnczrlwak.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/giwheobcf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/goafskqet.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gzyswcfmb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gamsdzyrp.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gdsrcxmlr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gaichzmat.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gchrtghfk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gcivtqyka.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gzxafptli.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/guskxaelj.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gxilksbui.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gdkcuzvjb.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gadlqefxb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gkrkbkffn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/goeqitrww.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gqzgcsvfl.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gwpigmcvc.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gwevwtoih.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gvrlbkaxh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gykslgfsz.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gecmfrmte.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gyczojlkg.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/geoqyvblq.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gdlzcrtmh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gbkwfwald.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/gmbpvhdgq.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gnqmjbrlr.sHtML


<!-- 参考信息 -->