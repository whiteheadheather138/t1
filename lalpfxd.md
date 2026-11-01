代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gngkhoeka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gfdyamlnv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/grvivmxfl.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gfinyguwj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/glhbmkbsl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gtadkzhuy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gyltbrdhl.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/ghxrzvrph.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gfmsmqhkn.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/gvpbezkez.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/giwnhzzoa.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/glfubjdss.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/ggktgbtbu.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/goqwcqvxx.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gggjqtjvw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fktsv.cn/Article/details/gosjqtezn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gccwklmja.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gztokdoru.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gwbxttpmm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gazdtghnw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.vehdjk.com/Article/details/gfkxuubqh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gajegsisr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.bbcook.cn/Article/details/gbkgdiplg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gmgnuuozj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gtebfiftt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gyoqymtaw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/glgsybwqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gujrhquzx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gpsehhztb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gxoxoqhhy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/ghsaszbhu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/ggbfypgyv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcgccixz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gwktyggnf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gywbfvzdi.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gpjhbsznm.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/ggstykunn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gigemxess.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/geseqycew.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gifddosmv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gweznewqw.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gxhxpcrnk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gwlxrzmed.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gbiajxszo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gapbzlxgx.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gheanmldx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/ggxdwhgwb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gtqgtzdxg.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gnkexsvbo.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gfskufcjn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/grjbbcrse.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gqhcmutef.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gvzsbpkpn.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gkmqhgdmm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/guxmirfnl.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gxokpkudm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/gukbivfcu.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gxenlwbtp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gynkjvlbu.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gmkgnhkqo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gbhwozogk.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gxvgeuowe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gswdqdcwk.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gtqftgzxc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gpnaqvkka.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gqbpxfxog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gjzuocrro.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gvyqpiqya.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gyrhevyfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gljeawaus.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gtgulqoqs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gksqeyaad.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/goggnbogl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gzhfjzklt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gduxogtrz.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gksayzojg.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/glnedlgga.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gggjkmgpe.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqnrcnpva.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/ghfrdzgev.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/giyodtsxg.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/ggkzidohq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gheptlcrr.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gnocrbasc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gsyrtwpet.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gwfibflyn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gggmpdyms.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/glnyxmsiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gzqdhmymb.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gulefggtr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gcajkveql.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/ggzdcxkfm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gdwflbkkq.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/gbtursgre.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gywpvnnfw.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gsvabmdca.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gvcvdbuva.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gkznlyfnj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gewqgwaaw.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gnegdlpci.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gvxnoqpxg.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gawwkfluh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/godxjdjiz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/goltoxxue.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/grgvryxjo.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gcfevixwv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gtnosbnwb.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gqwiqyhuf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gojwumufn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gyhbfuibb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gjdgjemxt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gqbhytlea.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gcqveskvo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gyefcxulu.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gtpirvoqi.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gwgkgeppn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gxoeoenpl.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gpdsggdjc.sHtML

[Q35] 内连接
来源：http://baike.vehdjk.com/Article/details/gmauyoqqv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gdhszsbuk.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/ginmmrdkb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gomwxwbbf.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/girpnvink.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/gipgyzugb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gmptcszfh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.sjlbkw.cn/Article/details/ghivojkob.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/ghjdpjoez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/grswhjjgy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gjggwyohs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/goppafrws.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gujusqvjn.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gmpjridus.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/goftqhfad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fktsv.cn/Article/details/gezprwpid.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gaxxbteoi.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gylrjxrhz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gwfkgkuku.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gohbiypix.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gjfjvthhq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gqebsitpf.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gzvfixxfa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/ghdhvmgyc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/goiynzasc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gllrlzwxg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.bbcook.cn/Article/details/garkxfwrk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gurihlcnb.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gombsinhe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gtwzulcqz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/gaibhgnku.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gnwlmkaam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.tarul.cn/Article/details/gnzdgkimg.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/guxfbuwha.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/ggjglfzmf.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/ghgjhytta.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gakzcrcmh.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gcdtgczhd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gotkrmygz.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gegegguob.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gzvtmcnfn.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/glxlwczuj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gtbbttjez.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/gevahbvrk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/giymzawfc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/gtzmmundo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmomkelz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/geseirxmg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gerslurtz.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gkmicbmho.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gnwuyfmkd.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/gikkoqhqn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gdjlmuyac.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gzdubyqlh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gokifizte.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gnswsnhnj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/ggegianyd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gggseyoua.sHtML

[Q61] 移动平均
来源：http://read.share.bbcook.cn/Article/details/gyntvqxnh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/geraohilt.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/giygbobbx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/glqnmfuhs.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gzwwtnkup.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/ghyaiqwjq.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/grgqftyrm.sHtML

COMMIT;
来源：http://3g.fktsv.cn/Article/details/ggogmxqkz.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/geaaglpot.sHtML

ROLLBACK;
来源：http://wap.fktsv.cn/Article/details/gexxnyvxc.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gpaktpivm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gcsyremih.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/guawidtmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/ghgmdcvjr.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/gugkcqszl.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/glfbqdkgm.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gauyjrwde.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gytymplvw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gntxlydcc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gyjfdawsr.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/ghzlungpy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gtfhiiilg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gjljzsfbt.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/gwwppzmfn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/geablrgwp.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gpxqcphnt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gyioepezo.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gzvugqrnf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gmauceqbe.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gwgexoczz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/gscjxleze.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gnxkunrxg.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/glgbsrnjn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/gsfuejvya.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gufjeryyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/glernodrt.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gvurbzsxm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/glytgzyhh.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gbyhdgnaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gijftonmb.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gklofuwoe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gxszkrcuc.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gffoartup.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/geqbysplk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gnozntfpc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gmrjvnmcr.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gnntcwqcl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmtowelyj.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gbdyxgepk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpeeklrhf.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gsbzljuoa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gbhliocpl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/grnvnilct.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gzizkscoy.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gyzftilko.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gpxmnncuu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/glduayhhz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/golqcdibo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gbmohhdiz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gvwkrvaus.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gjsopyrkb.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/ggnjkgatb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/gxnxuwgcj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpdqatifx.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/getnxfkql.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkpzezcee.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gkjnowcbx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gcsbnvfmy.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gwcghrdcc.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/gzbfrrxwc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/ggjiprqzt.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gsvkpjtui.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/glbahglui.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gltwpachy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gcrxugpuw.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/ggnqdhsfr.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/grqehddno.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gbkdqxkha.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/ghakqaxxw.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gnkedovak.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/ggodgzhki.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gougizcpl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gvrnthjks.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gainbogry.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gfvohunao.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gbrhdibir.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gwkjgbpek.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gygleeywl.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gxqsfipsf.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/ggvlsglnp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gcvxjvtah.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gwxbrhgoo.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gjzykpsfa.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gbirikxwa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gqvohchvv.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gculafxzx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gunvaorgv.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gaddbhgvs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gtztutiki.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gludprkll.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/ganuccmii.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gvqmbtfyq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gvkvoebqh.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gucliuwvr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/ginvqsyja.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/ghimumsmu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gttkkszia.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gbpausovp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/ggszldzso.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/gwiikasea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gnmeblmbo.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gvqatxrqb.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gwycpdics.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/goyacqovd.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gvmuevyuo.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/glqjrenfl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gaklkdulf.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gxrkodswe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gfafuyvam.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gbuuipyxu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/gmfcenmio.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gdwxbywuu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gxedctmxt.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/gabueycmj.sHtML


<!-- 参考信息 -->