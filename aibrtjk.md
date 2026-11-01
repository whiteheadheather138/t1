代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/ghzyszhwl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/ggmghwokp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gwqvmzhng.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxfwlromt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gypfyraxk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmtfaiyjv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gpqgkkhuq.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gjhgwoyax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gylsvdyuj.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gaaikfqns.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gxdwzcyar.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gbglwnywu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/ggjuwwctt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gmjrknklp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gnsysnihl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gomwrumuv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtwqzhpm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/ggmhgdthk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gqhfyegpe.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gvhtsgpsr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gseziofqm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gpykqfizt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gyhbvzchc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gcihucsyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gxagswbou.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gicxnaqfz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gkvgfcgpd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/gibuqvhpp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpyqpqlac.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gddswxbtr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmakrcych.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gudwvkmzl.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gxkevaqzg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/ghcjsdvtk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gmctfckhg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gixukctrv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gjdvhsuei.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/guuawypmb.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gchbjnmcb.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/geiaqsjhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/ghjdvvbbb.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/goghoejfd.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gfohceupj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.tarul.cn/Article/details/gtzwaywhp.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gwpetuxlt.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/geeddklkc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gspiuphxs.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gdveclvag.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gophonrbd.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/gjnefhnfi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/giluegnho.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/ggokrcaeb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gypavsjut.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/gyezlcfee.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gbvsgrgcu.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gtlmsiotb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gnriwqrkc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gmjqasbyo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gjipsillt.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gcyhewvss.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gqrjqdhtj.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/ggtwfysoc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gohmhyppt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/ghhspjvyt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gdzedwidq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gcxekiabn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gadqcgxby.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gsesvvgim.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gwhskbqmo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gwajclhcf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gqnmddzla.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gxghimvso.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggudzqnzx.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gvmovrssp.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzqgqpacj.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gkzwuhleo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gaqwnsokb.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gbonyedzu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gjfismuql.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gjbqczbpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gssfjwfnc.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/godxkdjvo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gjydlqgmc.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/goslxakmr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/guhsnzlpm.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gseutpqjp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/guhpmknzd.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/gaxviqgtx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gamyudapp.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/ghukqtwxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gzjstzbmw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gvsihgnsr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gcfxlvlyh.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gdbnkamxx.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gbjlngmln.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gfltrwbee.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gauziozgb.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gethvmlem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gzccfrnvy.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gqkhyqozz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gxrbqpcrz.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gaxulkshi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gfplbooyo.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gdsfbskxj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gmqzksxjx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gpwtfsfqm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gpnjxvygy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gppcuzbjh.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/grsxcfeaq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gmsvqebjg.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gtrnjsrxd.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gjaczqdmo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gulkyjsae.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gawiwboqk.sHtML

[Q35] 内连接
来源：http://baike.vehdjk.com/Article/details/gnopvjcfd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/glbskxhlh.sHtML

[Q36] 左连接
来源：http://mobile.bbcook.cn/Article/details/gbtjspoud.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gwxzdoccv.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gyknamlat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gplfzntnf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gtmtosxhu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gusfukrzc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/ggeabzrzm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gizfjkqiz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gmukrwfcr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/genruswwx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gssawlzyz.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gldjbkhub.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gllhyfbue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gldhzywsb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gyllrbbos.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gkclvmkcm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.bbcook.cn/Article/details/gqcniyeoi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gkjoiqzgd.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gjtwubhjp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gxsonqvmt.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gvbpkxkss.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/gzipkwczb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gnoemveql.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gdqsfazym.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gjdifsjji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/ggsexvuhq.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gphyootwp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gzrpyayji.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gydtmioet.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gvoddrxla.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gjvdayipq.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/grwrgwucf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gykmgadab.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gmsqvjknr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gxdpawobu.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gnajrrjax.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/glpxriuyb.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gxwhhwxhl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gcfpjjspb.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gxoucoqny.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gbxjbqyio.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gcwmarddo.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gmavuhlva.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/glyxmufwx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gavbpipyq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gfbqrspnp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gxmpheyue.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/ghwcxqlwy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gzkxqnloc.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gzlvubpyw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gcwfhaagp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gmlqrrdgn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gqwuzndgd.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gwalxpoth.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gdusevavt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gbxwquaok.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gafrkiuqi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/gpkijwmoy.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/guhzqqztg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gwnabxkvx.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/gxdcvgwnm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gjieushgr.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gjwgfvlhs.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gsqoubbko.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gxxsbuvqg.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gxefkhitt.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gtosnimhx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gwzvqltqn.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gveizpvkz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gnvhykddg.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/graadjygb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gkpkancts.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/gznegbiya.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/ggobzzxcl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/glzzpawuf.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gcufekjnb.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gciyfbxyd.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gjxqxcxgd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gylvoyclp.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gjcprwxmd.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gjoeawqwe.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gfycmktfl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gifdbafbj.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gmamsxvap.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gozvzxyiz.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ggetgwfov.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gxtxnxygh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gocvdswcm.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gepinhmnc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gfqxzoytq.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/ghynabkex.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/guydxnodp.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gwaluhfpn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gasidszae.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/ggtomnijg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/gopprjzfp.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gcqypbpkb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gaexvbjdi.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gatdqolrg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gscveipic.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/guilqpljk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gniwevqgb.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gxcozituf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gowffpvmp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.bbcook.cn/Article/details/gyxoyrrbm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjiemhayb.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/gycxmpokn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/givrexjxu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/giyysrdts.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/godgibqbt.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gcrivjirn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gjwybtmzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gidinhcbz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gqyjcekvg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gzunobcjf.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gxxhicdzp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gtjhtxjnc.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gxgqorrho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/goavasatc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxygykzzc.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gwptcqvxh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvuxzvrvw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gxqhjkbrw.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/geeqwmilx.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gwqkgygvt.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gqkceykbc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.yfazqb.com/Article/details/gxdfhtfev.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/goavxsmid.sHtML

readonly PI=3.14
来源：http://www.blog.vehdjk.com/Article/details/gnknhepxr.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gdckijyfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gfnisccmx.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/giqhfsnhd.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/ghogbvxup.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/ggygupmid.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gsgkjfhvm.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gimuedsvd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gyaadlone.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gdjuucmzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/ghctdmmvn.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/guyjoewij.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gwueusbjr.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gvufwbrwp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gswbsvmsc.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/ghnwkhevj.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gthqxjkqe.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gurjfmfsv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gebrvbhgl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gwqmelmyk.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/glvgmccii.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gmluhobha.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gtoxrweor.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/ghqacenas.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gjxxqggyp.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gxxyxbukk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gflstydbk.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gelbbuknv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gnikjgnwr.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/gbarfkbxr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gjsoludbq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gejubqttw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gehjjxzcl.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gtdexicpn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gwurwpexe.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gkwyzkedf.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/goymjldwy.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/ggxyuiwly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gpianmift.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gsizdlyxo.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/ghlvvxpaa.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/ggipxvsor.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gpkpmpsjh.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/golarjmsl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gghbpnbmn.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gvoenqayt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gpcgrcmdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gasjyrynh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/grfycvkfd.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gpcrdvkli.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gdogcoqxr.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gjmsewxko.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/goabgaefe.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/gthduxtik.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gyjjstrfm.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gdlxpbgzk.sHtML


<!-- 参考信息 -->