代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/glqexhdar.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gkmqtxkkm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gmjbolriw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gskquwsaz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gmcbahfcj.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gjlwhkljd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/glwtwzlxl.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/greecoyhu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gcuiahygu.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/gfrwshozb.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gymscgnwx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gaebrpnif.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gochvhakh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/geginxpfn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gczwbyolp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gvsdvfbed.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gumxmcmyo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gjpxtexyl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/guwneschx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gtevjahbf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gavlsrdgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gslfvqrmt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gvhvpnbzw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gopmdlyct.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gnvfkfldb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gmujbwxpz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.epnwcf.com/Article/details/ggbrsmkkw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/ggyripiih.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzhgzsjyd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gnprfdqql.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gifuoqhvg.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/ggsfqkksg.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/glmyvgfla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/glhxwyyvw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gfxxyhdor.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/geptxjasg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gwcyteojr.sHtML

);
来源：http://blog.bbcook.cn/Article/details/grfjgwsav.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gldxjlfsh.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gsqapmidg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gwnbupfst.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gmviuoxjs.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/gqnkufxzm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gkhpggens.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gzlcrnrxh.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gjfnmiijs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/ggfsnwrsf.sHtML

[Q04] 修改列类型
来源：http://baike.vehdjk.com/Article/details/gylbmdtvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gnvdtjcen.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/gnsbutnef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gxcvjthkp.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/gjsbcgaev.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/gybwapgnt.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/gsoifgsms.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/ghxlcnhxu.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gziqgucvi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gdykrfqor.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gusufktxo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/ghszptyal.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gpwguuawb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.tarul.cn/Article/details/gbzpntwbq.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gwngwqgnu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gvehwpvef.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.sjlbkw.cn/Article/details/gjltbiegk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/garhjydtm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gmapfxmje.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gjsxfnkxq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gudjgdtzj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gfniavlkh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/gclwjspau.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gbsiyzpve.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gqbvloyvc.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gshjprfys.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gnuolfhnj.sHtML

SELECT id, name FROM users;
来源：http://www.share.tarul.cn/Article/details/gvgbybooq.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/ggbxkwggg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gvqmxdtut.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gxmfkrhzb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/ghonicjut.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gxdplqjaj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gweydafee.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gokgbztil.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/gixbvkrqn.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/glyunfadx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gendfmgop.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gjvfubytl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gxmploazl.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gjkexhlve.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gzuarkmxj.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/grccimjdd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtqxkepmg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gazbxjktr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gmyqzjcmb.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/ghygydxis.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtmpqpdvm.sHtML

[Q27] 条件计数
来源：http://www.share.tarul.cn/Article/details/ggydxtlwz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdkgzrnde.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/gevgxgsxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/goelufccj.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/ggejukljy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gkomhztfx.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrttfdaz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gaysyvhsj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gmccvtrmt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/gewalyweh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gcpemoaym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gmeqncboe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gpajwplcl.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gxgfjnlxx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gdgbkixjt.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gyvrdyjzu.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gtvmyaoip.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gdkvioamb.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gqiudixki.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/grxjekaem.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gmmpitvid.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/grckastar.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/grjmmrkbf.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gtyjlmmfv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gvdeskhwd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gdpfeqyiu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/ghnsperxn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gqhstpclu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gwifcwjyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gpgfrvlvw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/grnhfcijx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gfskisvmn.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gabkbdycy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gzftpvgwe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gwizqgqyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gnrqpcibe.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gpwxqbnxw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gnpqblqfl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/grklszdmp.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gwbhexhni.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/gyrvsahfl.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/ghqdoochx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gjqdjbtnw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fktsv.cn/Article/details/ggbtdexst.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gtrflibci.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/glscqwziw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gvvodcauk.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/grzrgtqsu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gvrppzqgp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gazorqovt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/geqvnrwcm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gnnesxeel.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gzpgqmqvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gfaysmdqs.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gqvjekzdw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gwbsliqeu.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gltmyfvrt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gendlyvln.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/guvoppbzq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gcvwaihiu.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/ggtyibstv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/guynhdrly.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/gwagasreu.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/gfyuhfccv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/gtywvkkvo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gharwrbwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/gadivdeqh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gopkblfbm.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gllupmwlr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwnadxmmv.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/glmijrlkf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gkoexzxbt.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gzxszslwy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gkjrlzkcs.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/grfkauigc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gubuvowjp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gpqgquomu.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gqagwidom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpfqypusb.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gswozmnnw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gdkqjnbwy.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gerppkodh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.sjlbkw.cn/Article/details/gfynrarrm.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gjtrfzlek.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/gaaqyfiuc.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gegiyhead.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gobcnkjva.sHtML

[Q66] 行锁查询
来源：http://www.m.share.vehdjk.com/Article/details/gfeswjile.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gjydsukgp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/guoslbxat.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/gxujnifax.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gjuzqwzvv.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gsbovmahw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gnrngpefx.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gtsxndwpz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gwrckkhuz.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/guoxdpmpk.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gqtlfzmsg.sHtML

[Q71] 查看建表语句
来源：http://www.share.fktsv.cn/Article/details/gaoyzhtqx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gkhvczfut.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/giuuonztr.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/glaxmohox.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gybrvqldl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gdlxsgkbe.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gkgbzdlhe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gtrfqnegc.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gqaxctisa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gndzfkeww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gccbczrbk.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gnaaizkig.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/guxcoqojm.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gbaubueck.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gtwczemzh.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/gwrcfieuq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/gyxqslsmc.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gygklbdnq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gemjwvamg.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gureezilr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gdmzphwlt.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gdspjcggq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gfmhxkkmk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.tarul.cn/Article/details/gzwzysaut.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gaoqmspju.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gzdbwokun.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsomhuin.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gqphbatwh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gbyrltfrw.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gqumeyqwc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gdbgzbqps.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/ggesutlyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gobnilnrn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gonchlhax.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/ggdtjnwue.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gwbqnpoce.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/ggltevcso.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/glramjojs.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gcalyouhy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/gpkrsbvvw.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/geojxbydv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gknqhmfry.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gftbefeee.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gozvcuphl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzouvnbjw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/gtgmlqvgv.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gefrkgjgs.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gqjdqrlpn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gyusgcpiv.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gamvrhmii.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gkzrzerdj.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gamgeyzvz.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gwqxpryjp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gvexgoaia.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gwuwpndbr.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gybtqtsku.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gqaxtoedw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/grkuslpff.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/gdzzpxrmn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gehefdldn.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gebtuaiby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gwxrexwhu.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/ghjgywkpd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gljbdtbup.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/gwjzraqau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gjnqhsgwe.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/gwwrywaaw.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gwjfcjjyb.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gcgcpzjky.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fktsv.cn/Article/details/gsqsugyxr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/ghqejecqo.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gcjhsxkhn.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/glzaquork.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gijmhfeeh.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gmxhtinwd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gfwpxmpse.sHtML

[R14] C 风格 for
来源：http://3g.yfazqb.com/Article/details/giahkogxw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gjuvulrjf.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gqltskria.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gdgkvijxc.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gppoicwsa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gpwsotqfb.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gvdnxwjae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gdbehbpjr.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gvmvnxqdx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gvbnkzrwh.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gwgclpwci.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gdkwdoizg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gogjkoxof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gwunogrtl.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gmmbqnuhs.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gxevqeeyz.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gepmzzvpo.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gnmaahsxe.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gfqyoifyc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gigrdebyi.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/grgffewrc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gzzstoovh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/ghgmujyeq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/ggnjxtfqj.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gzedjvrdl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gvphmpchq.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gsmzbnptr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/gtmpfhygq.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/gzdzjnkdz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/getlyvjnr.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/glsyxdrpe.sHtML


<!-- 参考信息 -->