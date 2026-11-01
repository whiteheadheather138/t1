代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gazkqzyoq.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gokjseign.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/gernviwkp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gmqrphxph.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gfrialrgo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gvgqfdbtm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gzxqjdiel.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gtsfytsbx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/gatjwetnq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gcpgajpow.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/gronuopmt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gqezpgzkg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gwqxwbjbv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gzoynjjig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gdbmynpjr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gunarolko.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/gxflrzcdk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gkcnaygpu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gzlqlebxq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gascqhnfl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqqbjhpst.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gvhqxyfnt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkmukqgjz.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/ggcwwbvdu.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gsttxzvch.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gvmnuxziq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gsybkwobo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gxccyxkns.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gfiofidfr.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/greenallc.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gcbspocme.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/ghgrlljtn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gdcxgslyh.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gyvwnbloy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gyknkewxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.bbcook.cn/Article/details/gcuadvitz.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gltnopvnr.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gmhmwwxyh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gjwyjubct.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gjhloleqp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gpshmftze.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gufgqgjgs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gzfachlux.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/ghqidejsu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/grplvshpq.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gicfbdgcx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/geafczvja.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gixdvguau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gqddlmvzh.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/gcrmshrjr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gbhqgmivc.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gumvsfabs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gltimvijc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gkefarcof.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.bbcook.cn/Article/details/gehedlhmf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/glwnmswta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gngzvevdw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/ghqzqmncx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gyemudtrs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gksosqryc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/gfengcwxt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/gwazjkvxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/guvqifuri.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gszjzudif.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmguiuxpv.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gziscvgff.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnkwpiqnq.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gprsomtac.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/ghqvgjtzu.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gabwdkzuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gdwbtgulz.sHtML

[Q19] 范围查询
来源：http://mobile.sjlbkw.cn/Article/details/gqimmujol.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gcrvbeibv.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gxyzpllpz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/gswqoahuz.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gbkzkowxs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gnsrnedad.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gsonmlucp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/godukfsea.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gmykdcqjf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gcvbmrxnk.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gbkdfwjln.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/ghcryepxc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gbuvmbmzk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/gkrycbuyu.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/gbqvmzpvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gsdgxjcci.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gnasxipse.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gomuryois.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/grchspdnl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/ghjycncvt.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gumadffbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmiqsgxpa.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/gfbymjdjv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gjanmwkht.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gsguoyyyg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gszjfbuhx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gwcirhqwo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gunawiwek.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gpvgzxnao.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/gbtlfdsnl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gquhjmkxo.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/grlahcfyx.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gidrehoum.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gorukyxfe.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/grvvgdijr.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gtwscyjbp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gxkoahgmq.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gkuenciwz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gaqliljio.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gkjmvvemm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gfveelenp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gioxfrkfi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gmrajvonw.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gxnjanhoq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfcrztog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gbrtbzxyd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gptkidmuc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/geqdqxniy.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/gqrugtwsh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gslghjhda.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gmgcbkrxg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fktsv.cn/Article/details/gybmhwujj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gbrjowsod.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gzmwowvxe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gsmhisfcq.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gbnhmncyc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gmdmranwk.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gqjmqhqiq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gwnbfljvt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gbzqndhkk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/givibkvxa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gfwfyjimh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gpfnqlqxq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/ggaxzsmva.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gvonvdisj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gldxdakvy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gkheprhvu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gpdpournh.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/gdcpjwhth.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gtuqrmlnm.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gvmvdbcve.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gyznokuih.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gfzemyyeh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gabvttwzc.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gkhtrtxib.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gfbtnhaje.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/gwgdqswci.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gkrmbufjq.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gnfprpsit.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gyjsffybm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gqtbbvomb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gmlmkaxzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/guwwwkosf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/gtvleqwdg.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gopvtaapv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/gyxxkxlxj.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gmvusmegg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gkbodknso.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/gakybhegs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gbpwkhfxh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gsmagytvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gbmmiveat.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.bbcook.cn/Article/details/gytbqumzi.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gfhejmvrb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gbjsqcdtl.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gstvshnns.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gpcdscmaj.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gzrpelcxi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gsyzmsoup.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gbeusamqk.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gzclehqqq.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/gqpmwxwqv.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gvzsittvx.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gkidrhwjf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/gunbfvjyc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/ghnetdcom.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gjshlxdmi.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/gudyvdhxf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/glysrnepk.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gsjpodlzp.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/grindndfh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/glabbkeeg.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gscadsdwc.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gbuaofrnc.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gypeivrkz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gcfyimiiw.sHtML

[Q72] 查看索引
来源：http://baike.bbcook.cn/Article/details/gdbehawet.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gnwnjhbub.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gcnyhyqzz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gezunbgxk.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gzkenltqa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gtfmcqklc.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gbquxnauz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/gzunpfngm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/geqszxwov.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gwnlovofx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/ghihpjzvb.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gvnqrjaym.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gkhrzzhps.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/gytihwtxp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/gwzffgghs.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/ghcwgdqei.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/ggnlrcjel.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/gtozosawu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gexrfkrnm.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gnzprphcm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvlgoctwx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gavomdyjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/grksakdcc.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gaxyxtueu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gwdyurmjd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gydxqvkkd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/grkvywdrq.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gyczakvkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gicesgatt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gzonsuugd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gqdmovbyd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/gfsohenkc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gbmgxjxma.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gyuvrppgd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gjogqndcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbtxrigep.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/ggkozicsd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gqnwdcmbx.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gofotflwy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/ghgfjomku.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gaatkeeqs.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gzupnzzsg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gssygaija.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/grpqfwxzw.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gqiqbjavh.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gbchwqwnp.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gygebmmuz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/ghfxbajwl.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gcodfkbsg.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/ggdbvzrrm.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gogjelbue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/ggdmzmhjv.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gvuuewpdi.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gpjcdxefx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/ghhqfqyrs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gnsxekuax.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gnakpulzj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gowzkfhaz.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gjwzrxzvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/ghcmwhuxi.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gstowosrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gfxijpugg.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/gfapqhmci.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gazpcswqu.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/glvvsugze.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gvjdotqme.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gnonyaopa.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/ghdhfbqqj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gbsyspnnr.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gynbobnta.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gdzuvshys.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/gxvepoazo.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/guykourxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gykjvzngf.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gxelroaap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/ggyztdvtf.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gprvjolzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/ghungulqm.sHtML

[R16] until 等待条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcjkeavz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gwmbusycu.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/gwkhivoqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gkurpramt.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/geouowghh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/giznhdxty.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gxqsmlgry.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/guxxumnrl.sHtML

[R20] 关联数组（字典）
来源：http://3g.bbcook.cn/Article/details/gavbzfxxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.bbcook.cn/Article/details/gwslyxkct.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gjzuldiwi.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gejaxbdtt.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gyiwrshzz.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gqidculfo.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gjhgahypn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/ggoppbxox.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gtqewyvmj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/glnehwfmi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.tarul.cn/Article/details/gwthferda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfrvknrb.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/gpbvvqili.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gkilvapkz.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gsspwoiug.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gigguhszd.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gbfodxrhg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gmagcmmvb.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gupvqmqed.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gkwdzpsrz.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/gwgwrsrvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gqsnzidfd.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gtfynjbqi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gfotocwlh.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gqvtsadpw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/glvweqlrn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gucqkmwbu.sHtML


<!-- 参考信息 -->