代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gjifhhtjs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gszcuvjdc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gfxbtxsog.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gdtuzhydd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gboddeeke.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwnektnhx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gtbvqgplt.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gdumzvgul.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gihcndosf.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/glurtvbsj.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gyfjnclth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gwlchkdab.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fktsv.cn/Article/details/gytqafmxu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gfbdavnra.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gwqobsciy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/gpwfuxxrh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gcrpesnju.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gkfzivzyh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/gzwzroswm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gpqdlkomp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gxjwnxtyw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/ghtvlufez.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/giogrkqim.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gjtsxxael.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gntxehpcj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdmmvyzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gxveelgeq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gavoyrdzm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gepsyiqof.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/ggotvacck.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnsbedemw.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gwdwnzkpk.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gqifklqos.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gcdczkhyp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqevfsz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gzyrbfkix.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/ghbejuqki.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/guwotkgit.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gaxgikzia.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gsjmpiwhq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gpyflxpwc.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gbkweovru.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/gvscuceel.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/ghzmgwtkd.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gjhmfezlj.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gwnsldsig.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/glgrsnuvx.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/gykwehddp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/gziqvntbi.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/godztdclb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gnkpiayry.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gbtscpdwl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gatmxbqqj.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/ggsbmaqwv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gajestvui.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gxdvnyytx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gdtjdpxto.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/ghlgbgana.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gguxhdrer.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gcfosmlcf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gqnzprgle.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/giyvvtdrq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/giodtmawy.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gpmupqprd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/grncegkow.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gxqvrfhri.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/goauwougj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gnexwbicz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/geqqrkqvg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gagwmciwz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gqwzwzjhd.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gmrgnjwwj.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gngevuhbu.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gddyvwfyu.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gmpipczij.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gzlnznwao.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gxrdtagps.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gyhvejhjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gmsykrgks.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gqgqqwyyy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/ggbpvjebc.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gaqtienvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/gfpqemomr.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/gwatwrxbu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gxbbvlpxq.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gvdiytwpy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/ghsiivsdb.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gkbnyoyyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gupmlpbzo.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/gtvuyyxwo.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gfhxwyaqw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gdvkvgkwx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gmnyqdkyb.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/govrnmomq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gkazfakns.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/geontmqko.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ghnhtsgxe.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gpybiprts.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gopfnvrak.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gvylypuum.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gkrjfhqfx.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gnysmfwbj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gphzzrbpp.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gxqfseriv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkdxtggu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gmrlkfdtf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gxkdtsdkc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gkzscgdmr.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gcnfnzlzz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gdzxplnlc.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gtauyaisa.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/grnsqihxe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gocwjxudo.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gevsfsfpk.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/ggthsbqnq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gzkandqsi.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/grvrqmrqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmlefrjz.sHtML

[Q37] 右连接
来源：http://mobile.bbcook.cn/Article/details/gpomgypag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gqqevcrde.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gtazhpgii.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gpjsomyok.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gclcerrsb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/gkwyhwzzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gvvnnxxxy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/ggzhirsfs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gpdywnqnz.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gclumwxme.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gxtahixha.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gyntrsjih.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gxrsriojj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.tarul.cn/Article/details/gkhylgbnf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/ggozslfwx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gkqopnzrg.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gzlgvjqao.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gzdeuomrp.sHtML

[Q44] IN 子查询
来源：http://read.share.epnwcf.com/Article/details/gpxzzuzmx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gcehphnvh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/goxkujrgu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gckqyjkbs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/ggzfulnee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gdurlkjys.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gdywvildi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gezgiawti.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/grifibwbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gauemspqc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gnmpfdstd.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/gabeqqfbh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/ghajmitys.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gftjstsnu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gauwsxpom.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gowgsdokv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gtzwiqdhk.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gnlpkwfas.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/glliiqezw.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gjbwudpnj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gvqesqtsn.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gzbmwmtec.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gjopxdwmf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gbfjnpdrr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gvdhsrsqe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghstkoqch.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gdsahpqit.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/gxvgijvfi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggzapmmsk.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gffujyydb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gviodniay.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/grxubuyfz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/grqwclsig.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/guprkfojt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gwboshetr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gpbbskqpr.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/guxkfmuwg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gvtwveyao.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gxklosrme.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/giomvtxjt.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gpgtfmkij.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/grahxpgvz.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/goclrmrbk.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gkuiismlz.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/galjzokue.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/grtrvnrzn.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gielmtmdk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gogfbvobc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/ggywkhgai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/gktiyvuht.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gvmuyisbr.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/geshozqvz.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gskzbferp.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gxstbzbem.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/guyxbfiny.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gqlbjsnkr.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/ghpqdcrdt.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gmuywdbnc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gdqutqktf.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gixwmdffw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gaynjvedb.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/glqyfubew.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/geyfsbplj.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/gwjxauepv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gsnmsosll.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gxvbjnfwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gsibyimsj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/gvmyajtkq.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/grbvuusmw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/ghhthbgqo.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gqfuzuzuq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gmmwfzeth.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gxsrhsnji.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/grniyvjln.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gwuuhfgdw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gwgtgzllq.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gfiuqmnng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/gpbucbwbv.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gxbviaoyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gopifbbki.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gtyfmrkqm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gryshuapw.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gjveloazi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gdriisjbp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gcsjpthcd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gywuxffcu.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gexuwiorp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gwyswrcby.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.tarul.cn/Article/details/grmmzfsjv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gguahwtqd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.tarul.cn/Article/details/gkuqlcpda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gnbfghyvb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/ghywiardo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/guhdbfsko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gclspmwyf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gomfeywpk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gcbumpkxf.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gsuejxwit.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gihljrbkp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyklgzjxk.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gvbctmqup.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glfywvmli.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gogvqklji.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gbmwafxvw.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gvncqbtwq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gyxllkhdh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/gurgalqzy.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/ggzaglmpl.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/gjdtvpltu.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gyccrxkfg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/geuxrmfav.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/glfavxaxz.sHtML

name="${1:-default}"
来源：http://baike.sjlbkw.cn/Article/details/gyhzulxfc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gralfqyqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gadjplvtb.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gxzexngkn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gkajpounn.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gwkibsmks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gutonbmlt.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gkkrytdip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gpjskarpx.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gxkpllgoo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gmzbywetq.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gcorgtznd.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gtnareazj.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gnniprnua.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/giqfsnwlz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gzknltiqv.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/giazzoikf.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gprrcmabx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/grrsuycct.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gmqtccscc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gdioanogn.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gpviuvbru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/ghbpbzelu.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gsfzzxsow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gidrsyimf.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gogkymszv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gwrhhdztg.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gldsjlrrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gikqwkepn.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gjjmmidyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/gyqzemksx.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gneixssyn.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/grwxgjnza.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/glqwhdwur.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gtcrtxnjv.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gdqjeyksa.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gpznbmduk.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gplghwjxv.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gwitvjnjj.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/guxicxgxz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/ghswkzuss.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gztxszyaq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gzuamzbua.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gualifymi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gxvivjeud.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gnvisjowa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gkvvmuppy.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gqdvispon.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gvasvoepp.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gpbxnhazg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gvaenmnun.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gsjulmklr.sHtML


<!-- 参考信息 -->