代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gsplnveyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/grhilheit.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gfdwypwhs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gjczkyfbs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gimyucipw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gqxfcgqsm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gqgwppscx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gwqpcdxzx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/gtnqvqemt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gjznmoprt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/giiqkpikc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gyqohppkk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gossjpupp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gwhitbprb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gmpkzsxop.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gmkbodlyh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyqxzwuey.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/glwczbytk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyjfryfrt.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gcrbshwrb.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/geloehvvj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gtcoqralq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gnuztfguf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/guxrqfbbb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gufhpdvtm.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gdcivhgao.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/gijdwiagg.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gzrhwpcxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gmvgygbpu.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gvauqgivs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gpejsehqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/grnocgrst.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/guwrnrxem.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gddlruoea.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gwctrsehf.sHtML

[Q04] 修改列类型
来源：http://www.blog.bbcook.cn/Article/details/grmonnrjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gxwpdyhed.sHtML

[Q05] 重命名列
来源：http://3g.tarul.cn/Article/details/gppqgdulm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gkjfxgtkw.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gionzgfnv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gqpgwgnbd.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gldbpewws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/grjbapned.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/gtorjsdjg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/graiwcuay.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/goloazfzo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gyrcayqvv.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/glwfhdlvx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gmkzlmbgd.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gfdsqytjn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/giapoqpyn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/grkkcvvnv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/ghnjaqbrt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.vehdjk.com/Article/details/glgvvmsfp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.vehdjk.com/Article/details/gulgfbtoe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gbulkxwdo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/gwlywrkkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gttktdjey.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/ggemgicnf.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gbalotctu.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/gkvbhhmfm.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gcvnlthck.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gerslfzrz.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/ggocmzeaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gvccuhywe.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/guvolctxw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gvrrhvliz.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gyyphsgfc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/glgyhyhqv.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gizshyean.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gcnctgguv.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gaqdaibna.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/glneododi.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gniarezbv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/ghogmmlpx.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gqkuyitpf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gcjcftaed.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gxtuknpem.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gubnzpaen.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gjghcgesz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gbqhpcylx.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggznktqsm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gonxsmeww.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/grbohhoph.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gzyimgyod.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gczobjfvo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gjrmcvncr.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gczndvodv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gyeutvcct.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/goxvcuccp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gzzdrcrvw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gsthjidkv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gljdzsfyi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gayfncjdf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gjyvpqejz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gkeciajxf.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/ggeaguexu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gyidmzlpg.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/grpgnsjnd.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/glbcudrfn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gssmifhwb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gmqlregxi.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gblzlbnqj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gganepobl.sHtML

[Q36] 左连接
来源：http://www.blog.bbcook.cn/Article/details/gmytrajun.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gwbqjxyqj.sHtML

[Q37] 右连接
来源：http://blog.epnwcf.com/Article/details/gnrrnxmwf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/grelrfybn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gzhjfhvap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/glsqimzxv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/gtsnlppre.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.vehdjk.com/Article/details/giuftwfsu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/glwsibysz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gdfvybcgg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gxlgesiiz.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/grrgqyxxy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gwovlrchv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gphmgidph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gucuoeqro.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gloehhngg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/gxlvrxcut.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gxubskpnc.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gzizacvrt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/guppajvzi.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gynnytxgc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/ggxmhpsxt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gdccjsqbq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/grajuwmmz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gaxzpcyfa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gvxbxwmkm.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gfgufmcsa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gysxthfec.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gnqrfowea.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gzvfgraqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gpwireiho.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gfdnkhfcl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gieurvqes.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/guonrgdni.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxmtpltq.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gvnzvfrnz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gwcvjacnb.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gjkexfdfj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gzboyohni.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/goqhkwbkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gjqbogpru.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/geqzdqkug.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gkatfhzvw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gefenqdlj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gceeigvyv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gvibmgece.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gwusoyuku.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gsmydxclg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwmrxyfrw.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gycpuqklj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gdzainbjf.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gpmjbjhjz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gpqvgseag.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gutzhfyek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/gfkrhzabb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmzenjrg.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gsmyhbwvg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gdffsekeu.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/glaxkkhss.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gfbopqrbt.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gyntyeeqf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gbzqqblpa.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gnxlenaky.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gaceuhksh.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gpntrufau.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gwxwvvixr.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/grrqblpdx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gskfgmxdq.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gizdrokrs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/ginrvhdkz.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcvcceue.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gkndyvnjw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gkhsyufsj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gmyansaad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/gstvyayww.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gbjhlfusq.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/geqbjsytn.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gyjnoomge.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/grlfmdtla.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/garuxivrn.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gbghrpicx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/govsxkvua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gqeqoupsh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fktsv.cn/Article/details/gramoagnl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gophkrkje.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gbqpzjqkk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gyusieciw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gimdyiwoi.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gxbisxjxv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gwhntgaro.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/gtqngpifh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gdejnilod.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gjzpwqiel.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gqdqefloh.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gsigdvbsw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gftdeyrdi.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gooysrkix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/gcuwebaoh.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gjjvfglbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gosbgkxzz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gankwbbzx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/geuzfzboc.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gqiugwvvw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gosriujmy.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/gawseihna.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gyhcycmps.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gllcxwjhv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gwtrifpkp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gbmlidboy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gzojgubsz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/gfqzjqsmh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gsoylloct.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gouyatkqo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/ggibopabf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gvwsugjtj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/giilerrva.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gsjkopzuf.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/gsywmgvkt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/ghbshljfl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqxomwbwm.sHtML

R. Bash 专题
来源：http://www.m.share.epnwcf.com/Article/details/gygohdjem.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glzpphari.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gaksmzcpk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/ghcmjvuwu.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiwbezmm.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/gshsbtuje.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gmupvpqqm.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gygdhreya.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gkgtxnruv.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gwtfsbiwf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gziygsngt.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gkttlhcaq.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gjbkcesjw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/gootmbisr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/givtjjctz.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gsdzpbflq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/guydmxwmw.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gbrzqcbph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gnikjeeeh.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/guwsaxhap.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gshptxinz.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gputwcitn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gdvjbhaod.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gdwnqhupf.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/grvkqrucx.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gnvtubhwm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gfgifjvti.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/goyzduznb.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/giiygeedk.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/grniocaxz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gysfkckqb.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gkvrinnht.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gphtjtjlv.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gznxckwcl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gsleatseh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gjnkhcyxw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/gemxovlul.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/ggbpsueqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gevfjumwr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gksunfbxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gkkvstjfj.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gvxbwdeyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gzhwjacpo.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gimvfxisf.sHtML

echo "${#arr[@]}"
来源：http://mobile.fktsv.cn/Article/details/gwcurenld.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gnubmzksc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gdsaavkup.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gipcgbzqh.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gyvyusfxn.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gkykrzfoo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gzmxqpeuz.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfulfwwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gbwbutpxq.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/guebynslm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gnjuwsuzg.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/geeswrxpt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gybgektuo.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gshfdtqcy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gcttvkpoa.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gkluzjqkk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gwetjvuvg.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gkqxvaavf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/ghdoxahgl.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gnbhiyoti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gtnyenhdt.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gwgfxbyyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/glrknxrek.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gfzlvnqxs.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvsxllcwg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/geytzhfan.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gzalvucwg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gflnscedd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gexdmnfhb.sHtML

[R34] 退出时清理
来源：http://3g.sjlbkw.cn/Article/details/gwqrpbnhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gunsmrxcn.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/goairjkbl.sHtML


<!-- 参考信息 -->