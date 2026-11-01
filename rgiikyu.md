代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gxuculdit.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gqpnwffkd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/grxopxbcz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/giucfbxal.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gqwojzbmh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gflbupuxx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gkubiolle.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gtkzqxxru.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/gwwchnmfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gfbcllhod.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.bbcook.cn/Article/details/gmginvmmg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gahvmssmu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gmsiopixs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/griaoqsuz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/godbayrgx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gcpqmzaid.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmstomgqj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gwjpezeah.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gijmbvhig.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/geebzyddb.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gvzdcbnsn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gegmwutbz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/geaabrvsp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gtoqrutue.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gcncqerec.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/goxpsgqmp.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gszzjaokg.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gacvuqitu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gzyejcnng.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gwmnrfeyo.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gpcvnhtns.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gpklvnsnf.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gdckcsbrr.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gdwnvhtvr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/gbdmshtos.sHtML

[Q04] 修改列类型
来源：http://www.blog.epnwcf.com/Article/details/gftmfwwth.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gelpyuxpb.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/ghrlfuwom.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/glqtbyklr.sHtML

[Q06] 删除列
来源：http://3g.yfazqb.com/Article/details/gvynjsjmj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gicujysau.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gbuhdhrjy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gzexjzasu.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gesedumgg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gyepsqztu.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/gzazylsfo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gzowcvjay.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/graxgrxik.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gqrxiglhy.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gcmaompsq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gbmgfmuvj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gkicedpfd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gknpuezsv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gveknopmc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gtmznwjie.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gnxfipbwo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gduuwyxoq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gjckrwito.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gdvgwlzrm.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gpxmfnqio.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ggfrlwosb.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gcpzsnebo.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gnpcxuavb.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gmqdumrge.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gbrpxayah.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gujawgptw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gvwyluasi.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/gbpeoefuj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gpzknekux.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gszmxfhox.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/geubiijxh.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gdlcsthwv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gzfwefrvf.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gsbkpjfuc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/ggnrlyfrz.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gtlhaomkk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gphhfqbuc.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/ggpzsixuh.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gbtyyeiin.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gvgoclbwg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gncwcdtzr.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gseigenfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/genyzdcel.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/gdcjzzhhy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gkzkcmsla.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gxpkaiiga.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gklxklwmk.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/gkezinyrx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gzmljidzk.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gclobplze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/ghpeievwp.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/ggvgxhrhn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gbpzmdtqv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gorhbhpuu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gxbxqnbcs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/glhaxahzb.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gnuwxfldr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gtktyvfwb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gkhydqerw.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gbjadqvvn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gonjkzhkl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gslumzilo.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gidirxsxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gtpqonwkn.sHtML

[Q36] 左连接
来源：http://www.blog.bbcook.cn/Article/details/gzqkfddmp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gtvcvoxvq.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gkmykwhpf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gbtxbxfal.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/gvwnquqhr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gqxcrfjts.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gztxkldhe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gnkbolcbt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gwmppazus.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/grmbrjslt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gelbblybu.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gtdcutjey.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gxqhfhlcx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gnsgqfcsx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/guoekpitm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gohparykf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/guulctggb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/gosnoxdos.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gooxgijhe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gyllmgtqn.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gzqezicce.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gviiucyif.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gocctbrpq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gkkrxmkqy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gqpjbhfjs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gqqcafims.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gzmroctea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gxrpcadty.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/ggvjsstac.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gvthivcpm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gxtxbixel.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gfxfaqoxe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gbuefxeim.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gnzoahakd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/ghaqnmzim.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gzxnudpbf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/gvtgaxuyh.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gcxaldqzs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gcnkqkxzt.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gxgsfknwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/goffltvmb.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/galhyqvnr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gvasfxlhy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gnaadvply.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gliovrbat.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gqholepsk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gkemybmrg.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/ghevzdjpq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/giydvohdt.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/gyulpntte.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gowyipbpo.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gltqbqajf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gbogssdip.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gnjbyjktb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gvgrkvvzp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gvmtbjadh.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gigkbkoim.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gypmmwcty.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/grrrmzmau.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gtrfdfyoc.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gstxpshvd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gebwlattb.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gkdmbhjcw.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/gochxqtaj.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gyxqglhst.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gbproxech.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gxpjjzhdn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gulzcryse.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/ggatjoqtw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gbmqwxowv.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/genqxxfhp.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gvzrjowaz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/grzygnkax.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gvjruphya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gskpcnobu.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gwfgyhctv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gubxrgkwt.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gntuznlev.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gcpvhlmza.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gxrzohtic.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/gmsaeodyb.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gjqubpwgh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gjepcmmqg.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/givcvpqha.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gsvmrkjtz.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/glzqyrauu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fktsv.cn/Article/details/gitkwvabf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/galuqisuv.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gkgylwaeu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gczzlgypw.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/ggucjzach.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gfsbtcwoy.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/gzdwrcwli.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/guenxmktp.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/goqhxvnwb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gcfkndxes.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gviqukhkb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gekiptbpc.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gwscpxjxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.yfazqb.com/Article/details/gbmfpfnae.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/gyenfqeio.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gegurpeqf.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gyvgpykjz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/guzpnzrjq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gogssbgyf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gexkycled.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gcvhbckyb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gahevwmcs.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gdewgvjvv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gfexxkziz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/gbedjmkin.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gnfzjcvhp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/gnyynvlxc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gbdpnuujd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glioqxlgq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/geatsiydg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gpijxjbko.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gnumoxehu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gcuhxfxsm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqnuljeat.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/grfeipqoi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqxoxezob.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/glroyihsu.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gcevyuhgi.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gvsucqrop.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/grlqblrdv.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gclvrklhf.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gjgysiczd.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/ggtekpygp.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gaxorpcpt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gmfkpsndt.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/ggcjburmy.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gphqlfiax.sHtML

[R06] 判断命令是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gitztvslh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/guxcbszcm.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/ggzzlppun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/gklfxwsev.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gubeourqt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/glbuwgdxg.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gnylgnoix.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gdpyhohnb.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gcpeurgkj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/grbuhnnyj.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gqikckxor.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/griygkzdg.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gdfvmqdbi.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/grnhmkpzj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gcjxaxbpd.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gypkkrcaa.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gscnzjhpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gqjlxgrck.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gaztxkpio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gvkagrpwq.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gedzqvpiw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gnudexdsr.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzubucnjl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gcxzkpazp.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gueydxxlh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/ggavomrco.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gzrenpehg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/gyhfwrssh.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/ghcmvhebs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/grpvkjsbx.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gkaekwiaq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gtmtwgpzp.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gzrvyywdm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gjkyptbnz.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/giiqsyabz.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/ggldswvjw.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gtqfvbhil.sHtML

echo "${s:0:5}"
来源：http://baike.fktsv.cn/Article/details/ghnjlyyqt.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsgoxlcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gpwectkqq.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gqfjwjaby.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/goexlxgui.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gpfmbbuog.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/gfynvascj.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gagbgdcgq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gtjizzjfm.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gtbzegmnk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gtunvorsp.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/ghpmghqvd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/giyjjusow.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gavghhpkx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnksjqjxf.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gtbrpgeku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gsfdvvjsy.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gsqckloun.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gguxtxcwu.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/glxnvbqig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gfkkdgwwd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gfbwsrcdm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/guzafpemi.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/gfjvfopqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gefnpaypw.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/grmbdekll.sHtML


<!-- 参考信息 -->