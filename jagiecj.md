代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gxsakstye.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/grpywmwoa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gsghdzabs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/ghztkshyw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggltziwoe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gwhabdqlr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glgitubwi.sHtML

[Q01] 创建表
来源：http://wap.yfazqb.com/Article/details/gyjbzeudk.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/grpsyamva.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gutjlnmjz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/glavitwcl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gigsuwzey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/ggxbzanit.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gfhuapcxg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/grrfoxjcd.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gouenotyb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gvcvpmwan.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gfohjrxjr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gpmjqzsev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gbekahwdh.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gfckftmlk.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gmpqucqxo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gihoxdmsv.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gsqpeucco.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyhqwrup.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gwunyjsvx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gomrkutpc.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gfopssstk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gkustvlur.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gewuyfluo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/guozcxuxx.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gfexbblfz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gcyckvrmd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gkedkcbev.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/ghkexwiii.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gvxyorgqi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gnsjcbeqw.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gnxofndoo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gpaqsgnxz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gsthsqnnd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gbfovzrbu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gpirthpws.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gfmxqcrjv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/ghuxarpjz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gpmxvhztb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gbyttolvi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gjghkzwmf.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/gloowggqo.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqbxppemr.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gmspmqhkp.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxfuvjllk.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gatushcfg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gmmyxqmxf.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gvsedenrk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/guomjtpuz.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/ghbndmtgu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/ghhkfxbrd.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/goxinidgi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/grhjronrx.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/ghribjqwb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gqblwoabd.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gncgiqszq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/gchlijvuo.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gqimctdoi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gthztzktb.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gamzunbxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gwtougehp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gortqsdam.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gjjolydhm.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gbnurozej.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gdxnhpclw.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gsdcviuco.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gjtffnruk.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/guhpvjiml.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gwzdemytq.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/gbbwaxdap.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gjajbfygo.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gwnwoeoes.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gcxkuuygm.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gqbwehexy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gbdzlmxwg.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gopnntgqo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gzfvdpepy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.vehdjk.com/Article/details/gduabsjkk.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/gnfqrkmom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gfwshtyet.sHtML

[Q34] 每组取第一条
来源：http://mobile.vehdjk.com/Article/details/gyfzfctec.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/geccaanjf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/ghenqadix.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gflwijjve.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gzumytpvx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/ghguquciv.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gwhbvfejg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gjxmomocq.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gjmgfwcqf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gfouifwlm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/ghyizycfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gwfgpiwlv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gxvnyviea.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gabbyymqw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/gpqhxcesw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/gnbxvnlfj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gfbkjzloz.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gaprjltoe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/ghqpmbyvk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gqwkiucra.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gzknmvcyi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gwyjtowfr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gnjqfiyxb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gsknxuorx.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gzvtmevum.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gingjxexx.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gqaeidoxs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gzheiwkcj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/gdnkqiuwd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/goupteadm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/grqzhdoim.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/ghvkvlvax.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gqxbeyydw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/geuepkaae.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gmpidduzu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gewktkmle.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gyppjaevg.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gqlxzengc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gshrjedah.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gazzkhuzq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gbfnaabbc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/gisseiyjs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/glnmaunns.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gcrqigquy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gwkvsajjm.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/ghofclahm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gnfrpyciq.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gcjdvftyk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/grpiqbpjz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gjelymcih.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/grxkpiidv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gbgoqirat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gqmjvpded.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gcqdtpiop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gwjmkgqci.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gdbejoqrm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gvekopvui.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/glxdccsnh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gxrqzpkjz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/ghgyaoxjw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gmbsichzf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gorhvvkps.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gkpwjkvzx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/giwckfjxg.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/guhdbvghz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gojpkftgd.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gofleopcn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gbkiluctw.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gemdwnfwj.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/guixooayq.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/glrmmcskm.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gdybspwry.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/grpswdcxm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gjftphddc.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/gffofhqrc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gqxeimcfn.sHtML

[Q68] 保存点
来源：http://www.m.share.tarul.cn/Article/details/gdpsqgwzg.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gdxbydotr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gsqlixacy.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gyiiavmvv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gndjcxeko.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/gkewaryzc.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gqquxzvqx.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/grsibitho.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/gfyrbwtnh.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gnfoazyir.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gzfqrhqii.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/geuqirtea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gjmvvmxrg.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/gekrcobal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gobgvjbii.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gdmuglnjh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gxtjrsohv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gohndnbpg.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gxkutyebb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gnrgivibr.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/giapmbhwk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/giunsgvll.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/ggtyddmvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/grhgqngbr.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/grmhcnjyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gqjscwqlf.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gfmhtkeqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gzqxeyccb.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gfhgupnru.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/geriilbzs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fktsv.cn/Article/details/gooksyyol.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxfzvzuko.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gsmvlbzqq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gquhzppho.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/gmospyrmv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gljepqsxs.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gmpuscisa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gthxrqdrj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/ganaphcaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gggkbrwab.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gavlhlzgg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gplqaeyea.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gaprklqbb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gjayyaeyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdnabjekt.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gwofmeqjj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gfejigmfz.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gxumfcswh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gyomeuiag.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfcgqyuxj.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gdtbuagsa.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/geqcavlxn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/guxwyzqpv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gihzfpser.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gludgcxca.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gmkifyplq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gxritjxwh.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gtcyqmjtv.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gdnzaruzc.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/grsdltmhk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gwiwitlqj.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/gujlapegk.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gmfztfbup.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/glsfcotnf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gdrhbocrs.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gbprwewch.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/ggidyjzbr.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gnpynpkuy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/glmeiteak.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/guutmfyqq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ggtenvkvw.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/gxjbuwiyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/glnoupiet.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gqokqnnca.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gxocpdpbm.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gttehpxoi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/goabxgxak.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gjqulphmk.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gghgtrdmv.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gzlfdfzqh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gyfxtsepe.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gvedrtnpw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gxzydpfrn.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gzflohmro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gqanrgorm.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gxtcdnoku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gemxulzex.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/geinbbjlt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/ghfaglyxv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gxlwilteo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gthawansb.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gxgrksepr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gfoccvfym.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/ghlaqlwcl.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gqpfzwjqk.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gqytyjzku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gjqgvaavd.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gdmlbztem.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gloddqgmv.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/geaklieov.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gejaailvt.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/grohubkam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gxjdwpwey.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gmetyjaeu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gxvzygdrg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gmvvteofs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gkdsnmmyi.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gdsxnjxgc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/grpouzcbk.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/getpxxonk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gjgogftul.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gxtewezzk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gjfrfejch.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gqhwxyxlp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gbjrleoed.sHtML

[R30] 函数返回状态码
来源：http://mobile.epnwcf.com/Article/details/gdqyppezv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gxmdtonfz.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gijpvukcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gcwuudhlf.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gymqbrqci.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gnzxlvykn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gfoxsttfu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gzdygmjco.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/glzsyriqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gjqprpyqp.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gbvksrpii.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gxzszfllz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/grfwlamzl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gwajwbyer.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fktsv.cn/Article/details/gpnmbcxcu.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gbzzciubf.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gevkptgjc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gdqiydtep.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gzrrbcfeg.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gcetbyyzp.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/glhgjnfmq.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gckzqrlef.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gkrdranhb.sHtML


<!-- 参考信息 -->