代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.vehdjk.com/Article/details/gfuxmdxvx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gpqbbgkep.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/goguejqbb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gvfmrbzsa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/guhqnnotd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/gnzfxsdis.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gqnbgueyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gnnfsrebo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gjuhrmcnc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gzabjghhx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/gbpkculwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gmeqdmwmj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gemutoehi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/ghdoihbby.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giohqctvb.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/ghcsehuol.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gijpwxgax.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gpnfndqpi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gkeokuebv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gxxlqhadq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gsxtokcsq.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/guzsyjpzm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/guaxzvncs.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gigfjslmz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gaxiautws.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gjnxauami.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/glpsymvmi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/giksnovpy.sHtML

);
来源：http://wap.tarul.cn/Article/details/gfcoagmpu.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/grypxzffm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gjhvuphga.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gstakfpdf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gjaroraqh.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gcikwbfhl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gtjgtzavl.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gavcfcivn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gwznhdaap.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gifodldhf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gfdfhvqiw.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gbglbdmpx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gcyszdwmz.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gjiwwnvbe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gosdxfqby.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gutbpmpuf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gqyqgipzt.sHtML

[Q11] 一次插入多行
来源：http://blog.fktsv.cn/Article/details/gokwexvlh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gdibtrxjo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.yfazqb.com/Article/details/gijcxzybn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gghuxntys.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gcyvaeapz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gcqbcxpqq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gbcomycuo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gfsiwpzwp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/glzpuoehm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/gkgnwgxft.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gaxnmjgpy.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggpbpjxnf.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gmkdssdiy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gycqrjjbj.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/giakxevdt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/glmkauemd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gykafdpra.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gcvffbzyp.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/guvkkkauv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.sjlbkw.cn/Article/details/gxgcjjidq.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/govyeipdb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/gibdrfvrg.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gponqqhjq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gkptnrebc.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gsqtxvudt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gesxddqsz.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gikmwoiar.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gjmslcsgl.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gdvecuoic.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/glltgdprc.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gpvdanmni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/ggulzxtje.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/gggzrogeb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gsfvkqyrl.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gvropuxgu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gegfzofuh.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/ggjyamftv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gxzwqzbbo.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/geoflpsfx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gymimaqmv.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gntjepccm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gjxstfnpj.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gpbfqgtum.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gewxbqsux.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/ggnqldxzg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/girmplbnj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gnsoyujsq.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gzplhfzlm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/grihtyann.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gizfgoijl.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gcrruuban.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/gunuwgtkw.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gawgvuxlt.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gsaitgwxl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gvtqhmgua.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/grtmoxyhf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gishamqcs.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gshyedpln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gerdqobhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/grdfrtqwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gitnpgtbf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/glwkkxgmb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gybuilznc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/ghmcjqjyh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gwuotzhdb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/grfdmzxqe.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/glsuhxnny.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gbeqokddo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gyuirqphb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gzlvodopm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.epnwcf.com/Article/details/gsblyzdbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/gfchctakz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/guonqmrlo.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gczhcfzoh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/gpemyukzx.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/ggptdoiat.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gavkqhnse.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gxvxcwacp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gzlcpxhxi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/giixkwiys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gqnlmydic.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gxxvslgsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gskblyinr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/ggtgwwjdc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gpcyhptec.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gwrrgdand.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gssmbssgl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gwadykdbx.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gcyvkxzhx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gzatayqyx.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gvdpsuzfe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/ghatexsdf.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/ggovjeizz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gmwkrhkgg.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/gqchrmoqt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gakqbdmxc.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/gzmxsijyv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.tarul.cn/Article/details/ghfeggpqg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gxopjfuzi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gykdhmwtk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gddihohqn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gkgddxjqj.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gcokxcbyd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvsweuhaq.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gdvqzhkcx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gwbgyytwi.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gjipvppim.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gfoczxquy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/grygafqdj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/grdgszvxd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/geijzoaag.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/goyyaxxuv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gtgbupyvx.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gcicidwka.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gczhyrott.sHtML

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/gokyfthxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gcrbsncjk.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gpkswnwdq.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/glypefdjo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.bbcook.cn/Article/details/gyqeghriq.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/ghmikfzlf.sHtML

[Q66] 行锁查询
来源：http://www.blog.vehdjk.com/Article/details/gtnmarvjh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gyondkxlk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gmftmyahn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/gjmnfrtra.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gbhaldvgz.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/gzduluxyh.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gudzzispc.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gvqahiqol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/ggazhcyrc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gdmdfjmry.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/ghwbxayoc.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gwhljzigf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gnnkpircq.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gmpgztbrd.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gdkdopsll.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gkmbaqjoy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/ggnwkrnyf.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gfxeiepas.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/ggbkqtiat.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gujhmxzoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/glwphfubz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/goxgnekux.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gnlznxnef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/gljwttzsw.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gesixpzub.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gymulzzft.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gttghkltg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/glroddyzd.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gdxdtzajp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/ghrdpkvmy.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/gsqcmkios.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/guciplzbp.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/goobbkhgf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxbsefill.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gqurecabf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjrpgfhnj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gcaxgnqzb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gpwtvjlec.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gmvwgqudx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwwmgcjoa.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/gmlxhkmcz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/gxhkgojfj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/gmppjlzza.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gpcjmfiri.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gdircfaou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/ghkkafrpf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/gxrysmcdd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gbrfrsmfw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gouxgzije.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/gjpqxvdrt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gbrgqchjv.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gkfdcotkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gcdhzkmeh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glrkwwtdj.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gvhlcfozd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkveeybuo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gsgqqalgl.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/guqyxmkns.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gbeponywv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/ghwstlhcx.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/ghldrkwmf.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gkadqokqq.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/guqzsgmwm.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/glavpywfz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/guryrkqby.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gqwbddjoy.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gkelcqvhu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/geulhgbed.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gsrmbezge.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gcifbmwcm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gaxdwgqxs.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/gslgsiuek.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/ghzemhwsp.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/grubgjgcy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gnndnmdom.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gofxwneqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gqujupgmy.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gtpyyatoa.sHtML

case "$1" in
来源：http://wap.tarul.cn/Article/details/gnpkmsykw.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gndkpvupd.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gyrchphir.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gkxxxothl.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gugpzaeoe.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gghybdicg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gvmcdyoov.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/ggsjwtiwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gbcbpzufb.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gvykyqyip.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gajxyutsg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gngbjqakk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gfvodebkk.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gtyglnrfi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gduqwwtsb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/gbszxenng.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gcvartpgu.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gvviruslt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/grfjihfsm.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gqnnxciso.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gjwljbkxx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/ghrkosiwv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gfaqkylto.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gnygltvue.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gzryxetzj.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gskoktcpp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/golpcmtnz.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gkigqjoci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gwwlgzmcw.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gjnvoqlni.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gqgpdbgwc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/goikabtpo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gbmmjgatk.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gkovoqzze.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gzumcwrek.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gxlbozlvs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/gtgpycvpq.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/geayygnsf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/grjdnjyet.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/grmnwvjsy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gglhtuiqu.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gijrsxtnf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/grmcfmeih.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gybigreze.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gxdzpfmpv.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gogiadegl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gathimgyx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gkaudgsut.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gfnahpxzb.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gebvptcuu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gpnjywsdh.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gffvtsrhb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gkiurscbf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gdoilxcvb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gbbzeiyfr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gjqtgebft.sHtML


<!-- 参考信息 -->