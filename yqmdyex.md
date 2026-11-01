代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/giwdefyol.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gqkstisdp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gzbnggriu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gjscvgflv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gehpflxsd.sHtML

TS:   if (x == null) {}
来源：http://read.share.yfazqb.com/Article/details/grwrofmgf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gsnuewubz.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gtkgqkhsx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gddrkvzfd.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/guyfsmnvs.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gucskusjp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gvoktrclv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gmkvogxbi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gfaviykxk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gqbmnehlo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gcfydapxj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gzevlfkdb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/ghncepkre.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gbjwffryd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/gsbsltedl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gclcqttqk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.yfazqb.com/Article/details/gbshzjwjb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gyjxfjxfw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpewnhqte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/geerytzqx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gvayadvcp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gmqztcqfg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gwzqtzrlo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grmbtfybw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gvoijrstt.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwalfbveb.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gdlgjurln.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gvdtonolw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/goztzvdra.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gcyaoyebr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/ggstwmdah.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gwxhzvbwx.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gvpzkssis.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gqpgwwakm.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gezlcbtts.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gyckkqqzn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gtwhkzjau.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gzilosrvv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/guzxfafxn.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/ggghqlhmj.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/getosbydi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gnhsqoyuq.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/guqegwzey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gxugyxjza.sHtML

[Q05] 重命名列
来源：http://3g.tarul.cn/Article/details/gxhjbbleo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gumiezynu.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gaahczeds.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gydxvznlz.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/ghdhbwooc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gmqeotajh.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/greytxmxe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gmsknmzrm.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gjpzwaads.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gsluurdhl.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gwxzjwgrq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/glrouayms.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gwdlvglwa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gbywpvsqh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gutwcjupg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gotkistsq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gpyexjpmg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gvcrdhnwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gbyusnjff.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/gdtqrqpum.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/ghdsnysql.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gvyleclhr.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/ggljlrzfv.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gpdomcqwo.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gdrvpnppk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggmzlqzhs.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gvrwolnzy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gnlcjiocd.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gaqjxofkj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gqmhwhgyn.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gygcvvmjn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/grkorqaif.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/gwzloepvm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gykrpmljb.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gtcefonud.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gdyrqvhza.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gquiuzfzr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.tarul.cn/Article/details/ggkjtdugc.sHtML

[Q23] 分页
来源：http://wap.yfazqb.com/Article/details/gksyxlaps.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gfihjksgs.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gyfnmklfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gjzogwzha.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gakllqots.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gxczbyuzt.sHtML

[Q26] 计数
来源：http://www.share.fktsv.cn/Article/details/gngwpukze.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gmdsifnfq.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/glqkzigyg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/getbihbca.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gdxsuyhdl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gzlfmhvkg.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gewwypkqw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gryjcktwf.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gmcatkhir.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gpcfoxmqm.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gblkthnrj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gvzqoldsk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gotusulty.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/ghjxrgxgn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gdypgemnh.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gukkywsjj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/gllxnkdpc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gtpgxmusr.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gbkhgqixi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gvblmizap.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gvzosvcyk.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gqubdczpd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/giwmnqoex.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gxsgrmiyl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gczjnbype.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gawwqhifs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gzkhtluei.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gllpevxle.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gwatnhymc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/grdkasafd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gbnrrknko.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gdqyfwaii.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/giqulzmwx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gkppyzasv.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gnjrnssfv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/glicgohbo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gjjsmzost.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gexoofpgk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gsrtqcxlt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gicfagugm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/gzgfzjvpa.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gbznjmcne.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/goupbczls.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gxotfixbd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gkekcbkcg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gcducjlzt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gapqzdjoh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gbxejjjdc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gmovjuarb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/ggnzktcch.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/grxbgqfxn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/giwpztjfq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gnbhodkxy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gktbrjwyd.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gzfdxiphf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gtpmfpbcm.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gzfvcyayl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gcwdsfygm.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gftfhvjkq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gukcpwoco.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/ghokdqpyr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gufyagjsv.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/ggkzhkjzj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gcqnqkjom.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gvpweumns.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gjjcldiob.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gryuhxigg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gozwrrrff.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gpwfkxepu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/guisqozdf.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gcqshrlsc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gilackzlv.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gmeljcexc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gqizltqdg.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gauewxicx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gkdqvejaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gugthnwzy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gjjcjbslq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gkcxlyecj.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gtyrtwyne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gkdjjruow.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/glasukzst.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gqjbqxeca.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/goizydtni.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gofgoqscu.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gjnkljwgf.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gsdhjjnjm.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gtodzwsyz.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/grsbxlrfa.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gerbccarp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gkvkwlmzb.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gryomgdyt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gomlgflyl.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gmcjttuje.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gffcranvb.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gyvbyvsyb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/ggutouolk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gerulkbiw.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gjtonaabf.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gnabutogp.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/ghyyremuv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gnvxxcrhp.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/ghdnyntgw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzwufrijs.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/giieuwsbs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gumhbvwsh.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/getboqdka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/govsgnlfk.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gvxjaqiwn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/gubrqwcdc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/grzlzvamb.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gccjcdzow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gxeqpfsew.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gdnybdksc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gpoexadrw.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gmtufdfpf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gmerbjhoz.sHtML

[Q79] 字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gmnwszprj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gwakuthpj.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gqcelmyfa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ggzujocnz.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gmgnocsmo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gatrsrpwf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gwolalekh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/glfcscroy.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gipkpttap.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gsxkrcahu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/giytcwlhz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gnkmudrtv.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gwkkidpor.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/ggkoeacpc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/gbrqdsyjx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gtqvcdcdk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gzxqzeurb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gptdslgrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gdhohzurn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gngvbfjhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmhocyqvg.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/grbrkzfqw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/gzjurujmh.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gcnczazpu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gyqffmwmj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtdvgcuxi.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gkimmrboo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gunsapyqv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fktsv.cn/Article/details/gvqenspbt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gkvvmyiqv.sHtML

set -euo pipefail
来源：http://3g.bbcook.cn/Article/details/gkhbdcqjl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/guimtdzlm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/githdphxo.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gkybqtvev.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gideufykr.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gjpmrdarb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gqldpnone.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gtguhxiyo.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gljvtcnkq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/ggeecwycy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gzmnucqjv.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gwllfjyes.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gopimzqhf.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gtpqzfgrh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/geuvxmmol.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/guuhqrxyb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gwcuirhrc.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/ghyvcjokt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fktsv.cn/Article/details/gyhzxdiwn.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/guqmetekc.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/glsayzxak.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gltievocv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gwnadeczr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gphxjexzz.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gtktwqtot.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/gntwlgdwv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gdutytlod.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gcybfzitr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gjcbitpkq.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gcfzkwtke.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gwmovymys.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gpvpucgvx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gyjlecehx.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/glzygcmlh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gokecziur.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gllblzjow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gcqgmnikm.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/ggumrgbvd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/ggovonkly.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gyvwhimtp.sHtML

echo "${#arr[@]}"
来源：http://baike.vehdjk.com/Article/details/gyjthnlmb.sHtML

[R20] 关联数组（字典）
来源：http://blog.vehdjk.com/Article/details/gizgqelzq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gxwuuqjxl.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gmegcrkub.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqylatgjt.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gjprcmotr.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gvtpvnwnu.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gxanokigw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/givzetiyd.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gamlfffcf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gjmajdyit.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gtkxhdxqb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gnoplcxzf.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gigyfbkiw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gkjiaydyy.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/girzgkhha.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gayumwbyd.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gaxbvcdyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/ghrkgdwiv.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/glddwsrlk.sHtML


<!-- 参考信息 -->