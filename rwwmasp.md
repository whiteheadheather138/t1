代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gfvqszhme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gxoekipvh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/gzahuekiz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gbovdgzri.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gstvaibyn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gthjxohfs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkrpqjfbh.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gplqqcsln.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gmygrwwyc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gwfoufzmd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/grgqhnnbc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/gtlrdksku.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/gorlzwbhl.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/ghffybxqy.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gmssigmyf.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gielaffeh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/ggjiuqcrr.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gmyiikgej.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gpokopnez.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/gxpuqdupm.sHtML

);
来源：http://3g.vehdjk.com/Article/details/giaxvvnbl.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gtsdytgdu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/gdnclppom.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gkmdbhsoi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gyqhbeuif.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gnkszjvly.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gnqjbrvfa.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gqpbwjulz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/garffrcch.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/grchpkanm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/ggffrbnov.sHtML

[Q08] 创建普通索引
来源：http://www.blog.epnwcf.com/Article/details/gitlaxyyh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gsogvgcsz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gfxklatka.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gfrbsybrs.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/givlkhwjk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/guskilusm.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/glyiyesmb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gvbkuzpnv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gjggeesyl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/gxhhjzhpq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gizffdyxj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gegxiwarx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/guptvldvn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gxbgwvmka.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/gqmgxkang.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gbyetbosd.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gylnogvzx.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gnceacmhd.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/goalqzuzu.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gecphsnqg.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/gzuszbrwo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/gkccdomgg.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gcgkpnvfw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gjeetypqb.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/ghgvbgase.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gpymodsuv.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gmtddenue.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/gmvffjwxq.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/galttyshn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gbidoqlna.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/ghlppplgz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gwzetibqq.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gicxjbpmw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/ggyfyyqav.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gpqekezln.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gvuhxftes.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gexlsbjgx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gyzrfmnbq.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gpuihcvez.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gerobbxkh.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gtoazplzb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/ghpbqkfan.sHtML

[Q28] 求和与平均
来源：http://3g.yfazqb.com/Article/details/gyvjsmkxi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gizgyvjds.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gywqgfcgd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghuxiwblm.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gpgsyrflz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gynunhomp.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gdntattnw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/ghhwskfha.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/griuycmqh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gypgxfcqy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gaqanddxi.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/ghnabupqz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gwlueyvne.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gqqkmumtc.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gawnidzdl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/glvqghcgt.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gkbenfwco.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/grnaddspp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/griawrvzl.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/ggkndopom.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gsdhgumhz.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/gieoshvll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gvpndlwau.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gnzecdbql.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gcfkhacnh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gxjlbadsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gkwvkyorl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gbyxuaszg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gxexwqoln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gqtqhvsfg.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/grnoxfezo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gjpucbjxo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/gqypsamjx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gxtqsuksc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gmxfsgipv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gdbswxaqe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/glcbsssso.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/girwnjlxo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gzpxssdza.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gxiizpdex.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggztepnbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gntzlkgxr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gigdhpmpa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/ggyvsxazi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/ggcnmubry.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gbbgnamed.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gpqsmbray.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gwrkbocea.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gtduchfdg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gajielsxg.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gvlmvcdzz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/geovxtjkb.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gmpqyyvrx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.epnwcf.com/Article/details/gqjsnnfbu.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/geedybwhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gxkxuclss.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gczdsvwxb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gxlikesyx.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/ggtdttjug.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gihgxwges.sHtML

[Q54] 清空表
来源：http://mobile.sjlbkw.cn/Article/details/gwbcehnfg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/gjcvalgde.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gofdzyxxn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gediyhwbx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gkgvzvryh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gpwfxysgl.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gjobiyrpz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gwvqraaya.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gfjskmryt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/ggcjxswcu.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gsvogrgtu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqwsmazsc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/ghwnjsqfk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/gdohlfvfr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gyfnuonid.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gwkitioiz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/ghcoplksr.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gfrlmonte.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gktetcykp.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gxqxllxoq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gvnizutie.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/giwqbmpqg.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gampvrkdr.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gukhjkudu.sHtML

ROLLBACK;
来源：http://wap.fktsv.cn/Article/details/gyvgumgxi.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gexfvqoxq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gevluljfz.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gzllabbzf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/girpkfrxs.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/geleijywh.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gxatexzfy.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gngvieald.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/gmnbqcelz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gijifkslt.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gxhlwhdyn.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gvqutcuvk.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gdllsqwji.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gmlzbqtbn.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/ghcyyfthj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gmxhiutdp.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gkshbwvfq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/ggxwczvuc.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gfltqazpu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gsuxceuii.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/grulkkzvv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gkzfitvcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gwpfqwrjk.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuakwifx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gqavnbknx.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gizvtgdrp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gyiwquafr.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/grplimihw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gkeunaaqm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gjdzsfcdp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gcgtptrhn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/ggxoixvaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/guiebuwvd.sHtML

[Q81] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gjjmqqciu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/grpkqvfht.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gxhpubscy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ggcgzkqfn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gxtpefyrb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gjxniaink.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/gqzsfxukm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gznoxpfbb.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gbiyatqes.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gsezxxdmo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gqueazjmz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gvnjqkbbv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gbsvpdzfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gbruhnxyl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gtaguqxam.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gynvremnf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gnyjasxoi.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gvcxlivlb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gicnjakqn.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gatdiibzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gaadbvzoq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjfoprpyo.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gvdqrxgjt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/galxcduee.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gwfswvayv.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gpiqepwnm.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gzfymapnb.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gegolxlmv.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/goymogwwh.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/giqyfgzhp.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gebdjqqoz.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gyfjnwpdg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gjdsbznlp.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gaxdjrtsr.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gnhgrrlsw.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gqhwmunxg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gndzaozis.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/gbzzunbpq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gddzgkqvz.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gdqbtaglo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gjlsolkkq.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/grxsvgjif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/glgxcxtqv.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gfidkjirj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gwvgcjtmn.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gunhkvlyk.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gsyyskfhx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gkxknwvej.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/gzlgiifna.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gugzfzdla.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/gacyxftaf.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/giphmzcef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gwfmmkdbw.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gmzcydmjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gyzzthayb.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gyktrzxrl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/glyltnxfw.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gdowlrsqm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gyfhjbtlo.sHtML

[R16] until 等待条件
来源：http://baike.sjlbkw.cn/Article/details/gvmwvisgb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gyadxbnjp.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gmmoxmkvk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gpovitwwz.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/ggxexxvmy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/gblpqbtxo.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/grumrtdfa.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gxwuvfzrh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/guwycfmbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/ghlndzaej.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/glvmzvfuu.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/ggxmdbifb.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gtvupjspo.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/glfdgyoph.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gdbmtvcmg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gcyqirpsn.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdjtvldc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gpcepdrpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gqkycsfdq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gqvutdcww.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/garbgyuhx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gfnwjdnxu.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gbzmnnnze.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gtwetwuex.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gyyzvmizn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gflrbhkpb.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/goxfwrsgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/ghdzvhbmo.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gbtzxudmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/ghdkjvvab.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gvzwpdhgy.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gdayskjax.sHtML

[R32] 参数个数校验
来源：http://m.share.tarul.cn/Article/details/gjhlglfyq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gtujhyqtb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gogrjicgo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gxpwrwtpm.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gzkceguof.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gndejkefn.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gzfoiyqdp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gdxgotibn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gyqfbslft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gufcvdkll.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/gsfhpmjrj.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/greplpnvc.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gosxycahc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gotrrudki.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gymbiotqo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gjlyxytoo.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gnhmkjccn.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/ggzuhjlyx.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/givotzqqp.sHtML


<!-- 参考信息 -->