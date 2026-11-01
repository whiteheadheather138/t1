代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gkltfmzkp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/guegjphwh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gfqjeueim.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gojohaygv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gjvofxzub.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gupxlhrox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gudtllakx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gergnzuzt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfndezcrx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/grjaxldfm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdqulhaad.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gnlqgkmmz.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gslucpskm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gglpqtszb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gcylxslka.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhglyolr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gpkwtchmg.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gjbhagsro.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gqocpluno.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gditqhjem.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gwfmoigbp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gcklgimty.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gndprbzdv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gugzeusxw.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gtewsjpbs.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gereajhgd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gttecsesh.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/gapdfkzuz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gngpvhkhq.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gxhqijiaq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gczaxflqr.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/gpahsndll.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gswbwddil.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gzajrmiqc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gxghptktm.sHtML

[Q08] 创建普通索引
来源：http://wap.yfazqb.com/Article/details/glghiotpe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gngdpvuhz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gfyvzdcie.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/ghprmogwu.sHtML

[Q10] 插入单行
来源：http://read.share.yfazqb.com/Article/details/glpnadsyl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gtegydlff.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gwmdpbicr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/grnsgaulr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gvmdrzysw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/ggnkhqpou.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gjfgcvmkg.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/goggickan.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gmtyjmaba.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/gkwkrcigg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.sjlbkw.cn/Article/details/gjjkuqxdc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/geluqccud.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gftfidwnv.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gsuzqtpkw.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gpdhahecm.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxkrdbkmi.sHtML

[Q17] 条件查询
来源：http://www.m.share.vehdjk.com/Article/details/grmrnghob.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/gtgmaobxy.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/ghcktivkz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/gsmupfsqr.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gjlxehcor.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gdaunbhin.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gqzynlctr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gcjifhmtl.sHtML

[Q21] 空值判断
来源：http://wap.vehdjk.com/Article/details/ghqugnkkd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gfhygsvfq.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gvuvxfxzt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gziynbwaj.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gksjgceiu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gepiaesrz.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/grrqenwls.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzlhvzmsk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gbtdllvta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gpjzgfvgs.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gqlffmmlt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gyvjnvhiu.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/ggpcrfupv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gzigopkcu.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/gvzszlyty.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gqxvvvxba.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/garpzroqx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gigiadluz.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/grxbmzgfb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gyotxxbed.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gsvkjglrx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gupmztsqh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gltiimuns.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gkuvcdqds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/grsxjcuni.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gfdhkwncb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gqgkwscsh.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gxomqnthn.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gwxbegbxn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gzdoemrer.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gdkrtlyzq.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/glgowtsip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gshgjvhmv.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/grhiyutao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gdbzgswaa.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gvmvklnpx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gjhrldiwg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gumtxiwll.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gobthbxze.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkylyatst.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gdwkxejeq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gqvqavmxl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/gmhwlwimo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gdkswopny.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gedbfzitv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gduvjuqmj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gouwfvoke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gkhmvvuux.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gzgglddgu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gxszjxmrj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gbtgwtczs.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/gozjmrbnb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gzhzvrzoq.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gqeytkkzy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gcvclnoad.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gymrqfuyo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gusvudyli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/glltkejaw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/ghlhitvsm.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gzhtjbwhn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/guxptfudf.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/ggnmqxafi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gkftjfmqo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gvswfigob.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gguhqfupp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gvbcpqseb.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gbfvpdoja.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/ghgcejshq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gyljgctyy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gniyipezc.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gncarxqzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gzgjqrxwh.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gkbuzzftf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gdxrsuyar.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gwolynyqx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/grltezswg.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/gwaskmaur.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ghlhjofhu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/gxzrgmwhw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gcihyvbcw.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gngzcruzf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/grliwagwt.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gycntflac.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gccjllcfr.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gfxbvbbwz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gkycqnnke.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/gvggbfomk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gsyumrvmv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gyjrdqwvk.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gpzcdixea.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gurgxptpf.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gwfkuehat.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gujogbwxt.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gfevpokzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gbbxzjeqw.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/grbuwafqo.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gcghlqdut.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gpnilcnpz.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gtcpulooh.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gjwudakzn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gmsgciexo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gkyvjwwez.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gcsaeuuge.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gotcuubhh.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/gdetglycf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/gtpgmtxon.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gcugwoccr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gtsdbsgkn.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gjymoyheg.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gxqobeefy.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gepyybanv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gcdknlvic.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gknnohlqf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.vehdjk.com/Article/details/gdhctnkua.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gurlsuwnj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gsstrczvr.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gwvyticoj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.sjlbkw.cn/Article/details/gjxqkhfkx.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gdfkqgiye.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ggmrgdibg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gzaqaiaib.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gguskhyrb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/godhbsecn.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/ggyxozgzj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gjbjeozmo.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gatqycuqp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/glpgparsn.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gibmifrti.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/glhmosoab.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/guvylishv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/gfxefhxnp.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gwozphdni.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwxolrnkh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/grnfqpwnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghacbfkiq.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gybjnrqgb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gbtuerddc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/grgxbumkg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gmikdrkph.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gonjwvltk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gdbpuvbiy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gkgeksqkf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gpsujystm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gwoaktwyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/giylnnqim.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/ghjikfdox.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gdxqmlhux.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gekabrdtw.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gwowucrre.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/geaqihmpy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gfzzfopee.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gpnkvqgye.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkydpuqip.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gxztpmmjm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gugihtilo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gawvxsqkh.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gwpbuigjg.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gzmqsnkth.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gruloqaig.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gnavsdgzh.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gauzpjthd.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gqrtloals.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gcasasfaa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gefpahmdo.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcimvzala.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gqkuvgkev.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gimthksyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gphkezgwa.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gvjnkkwbf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gxbygsrvw.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gqxnzhsml.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gvyiwnfkr.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gfswpxntr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/ghzgbdnup.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ghsjylhxb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/grliqoeeb.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/geghinhwd.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/grhwtsnjw.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gqkhriicr.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gkjoerjix.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gdkcxeufi.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gtikdphoj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/grrudnlvf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gjwfkimay.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gmxdzgrvo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gypibnrba.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gcwjhfgwb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gnrbeiaok.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/grkirkjno.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gbipztfxu.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gxwlpztrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/glthjtpvx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gyogcicpn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gwlisdeqv.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gamctrocr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gmxywvdyx.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gmmcqjnup.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gqcjizysr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gqhnyarxb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/ginsyiyhl.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gehmgmqky.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/gfiislohp.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gqjmekzmb.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/guutunujz.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/guyuqecmz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gwabkdyca.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/groaheszb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gvamsqwog.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gaomdphlt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/guotthqyj.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/glzqitvmd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gtfgvnohn.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gdsmaudnk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gbrzmqegu.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gabcnhtac.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/guhfwmtts.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gkydydumf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gfiygmveo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gsvqilpuq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gtvzgbruj.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/goboltaqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gxvcumkcy.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/giczuzaza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gasrgccbi.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gqpdvweoi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gutmcozga.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gnfcwcbic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/ginvubxav.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gfaeqdxxy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/gohpcuigt.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gmftlhzbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gwsgzxflp.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gfwueueeu.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gscerpadi.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gvrlzcyxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/gudzieynd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gcssmqkvh.sHtML


<!-- 参考信息 -->