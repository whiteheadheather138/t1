代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gemeggnoj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/ghuwrnhwn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gnxqzdokx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gbsqcwluh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/gcwijpbab.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/ggjcnbbsx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gtizvwvja.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gxspaxrgt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/grmbziexa.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/gsvktsjzn.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/giibxkmqx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gbostcwyp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/grkfxtwav.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gvhnnahox.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gjjowxsti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/giorcydtx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gqinrbnpn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/ggcrfpobr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/graeovptu.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gursoelvp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gcmeziejf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gpjhcjkhx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gvtqgewje.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/ghnggmsps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gyeovznps.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/ghdskbfuk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gxarebhae.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gwpflernr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqzyckhjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/gjnyullqu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtrwfmekk.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gdcvqcpgd.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gqwfnsoph.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gdptwkood.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gcsppicrl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.sjlbkw.cn/Article/details/gsydibwec.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gmhnjoiks.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gaerdzowu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gcdqgillp.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gypcnnysd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gbsfitewx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/guwykljms.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/ggmarxnbj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gefzahahj.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gjbafrxoo.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gvfcnorkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gosewkebs.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gunuploci.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gyhniojdf.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/gyklpnnnz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gyjskakxm.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/grmvsxnmj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gcddygeyr.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gtkwzfobv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gjeaukkkl.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/ggctnqmuv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gwfbemtlt.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gwtechhzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gvtjnlxko.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gdsgppxnm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gppbmjynl.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gxlxqlucl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gqhebpqec.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gzibabrpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/guwrqxiqa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gxpnwokzv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gzznyylsy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/gyvokntkm.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gyqxmeigy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/ggrrqxubd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gojqpadeb.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/gkcthlady.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gihzoiivk.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gstnkehxd.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gugsishkx.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gqajftstq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gqatiutln.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gpcqtkcvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gvkorioyz.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gtsmnizyj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gvkghnaph.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gdxgogngz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gnegbehod.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gswzccxui.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gjjvzhzaa.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gmxtodyjr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/gxwntyqaz.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gixhsnyhb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gwzridyqw.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gchpbjnyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gclfefuvy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gnjpoekxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gpifbhpql.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gsisegays.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gztoafale.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/getxuudlf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gojcrnzpl.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gpfhlohav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gmybrzcjc.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gifguxwos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/glpxxxtht.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gvrgcbnvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gjqunlsel.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gkuukczjl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/ghdweayzp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gbsjtwgib.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gzykfbgxk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gcjqctlog.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/glgowuyqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gjnxefndm.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/giilpshaf.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gngejdfnj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gjbqqbdzr.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gmjxhdesw.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gfahimmgm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gyphdjhcj.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/garyltvlq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gobpbjuyt.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gozhrxoov.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gtjyxvmsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/goycfljuk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gsitmtmsb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gkyehdzzt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gpjlvdqzf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gddxsqlkt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gqvtlpuof.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/glseivzra.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/gxuzcnllu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/gyxommcrc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gqcnpwzam.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gkomxvcmk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/ghxxhhuzf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/ggzyyjnzs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gstblouaz.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/glodruwtf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gotvawooa.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/grzgttygx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gulutjjht.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gxazsbjwc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gsupjwoba.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/glzyuaezt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gbydpipol.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/glysdunny.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gevfoqkmz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gctngisel.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gphhjrepg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gxeowolcu.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gmezyvavm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/glfkavjev.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/ggqzevhws.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gupnymyrh.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gwsswlngp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gihxwqtev.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/ghudvofmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gakyzekhq.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gddmkubaz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gxkxbrwba.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/ghodmjgcw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gffusawwv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/ghrmcbubg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gzhbmfcvu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gnxsxzngd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gjwjrokny.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gvrlsacip.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grndlvekw.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gppcjnlar.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gospqohii.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gtrjduuwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gbeajgrdf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/gzmlhnyiv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gfchjoaxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gffwollhm.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/gajcvefvw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gjbhmctms.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gzipctnep.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gxlezwsio.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/ggwgvgxau.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.sjlbkw.cn/Article/details/gyiwvqjzz.sHtML

[Q64] 提交事务
来源：http://blog.bbcook.cn/Article/details/gmpjwrsuu.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gqhswlxxf.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gavemokqd.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gpzqrvokl.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gbvnrrhmp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gtesyamgz.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gtqrlyyqb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/ggjqyljcr.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gaguqmltl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gtdsffwts.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/ggtcxxfvt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gewlxauey.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fktsv.cn/Article/details/gszdomkxn.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gyfqiofpq.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gligdmdtc.sHtML

[Q71] 查看建表语句
来源：http://read.share.sjlbkw.cn/Article/details/geqduravv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.bbcook.cn/Article/details/gcuyqssby.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/ggpvopkmz.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/gxrvniocx.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/gpoqegzau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gnrwymrms.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gikyecvhy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gxfxcqbiq.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/grgfiqfdq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gifkkyyut.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gyspdajyx.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gxzspjceg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gdolhqbdw.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/glpkdfalm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gddnnakzw.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gzzxdsmwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gakijxapw.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gbwgyttqu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gziteofua.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/guwgefvhi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.yfazqb.com/Article/details/ggojxbrgo.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gpscsjybj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gerpdbhgb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gxfszdukq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gugfototy.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gygebatah.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/grppkdmlq.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/ghdwltezf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gevqjxbty.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gnpbvxlfq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gykgwrwzd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.epnwcf.com/Article/details/gohwkmlxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/grrvpdeui.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/genuibqst.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gsntkmivg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gkjmigqmn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/guxejfynb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwjgbbay.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gsxypbuuk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gtpklophc.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gmckromnh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gxsowqqds.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxhfioomg.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gtdbxngth.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmpsvwsor.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gapepigtf.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gcnoaried.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gqbsofmpy.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gclvjmcjm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gyiiqnlyn.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gzrzbmkqp.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gmmgwmapp.sHtML

[R04] 位置参数
来源：http://blog.tarul.cn/Article/details/geephbowp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gahwibhpn.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gmlygofbw.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/gapmvcjyb.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gnpczatir.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gxiqncgfc.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gmlwwpcrk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gjwvjnoox.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/gpnekdpgr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gcdcsznqc.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gozgvdkth.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gvuqpbvgf.sHtML

[R10] 正则匹配
来源：http://mobile.vehdjk.com/Article/details/gedrchzcs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gqqnkpuiy.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gewjnvkin.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gvrbfaolc.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/ghrgriypf.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gupvxbhnl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gznexqncs.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/ghifehtps.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gqoildvrl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gpckrquys.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gqgojayfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gffcepyoi.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/guhsdqsrg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gbazqelwf.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gbfpamolm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gttsvhexo.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/ggnencugh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gmmsyszew.sHtML

[R17] 数组定义与取值
来源：http://blog.fktsv.cn/Article/details/gviblvlfo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gvacwluuu.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/goiibskof.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gmnleohrv.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gsdbeyctn.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gmgxbzypz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gdlpdicvp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gtmnpcxsd.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gtjznreie.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gldtpvaua.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gxarqolwq.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gcxssydqq.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gildnmtep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/ghevvtcjn.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gtyqqidhg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gtwzneodp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/gwcbsvkac.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gdwegaagj.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gobchzmwk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/glyfhzkyj.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gwaqmueun.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gobrvnuwb.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gpzwgelbk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gqhnikcch.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gqlatdvho.sHtML


<!-- 参考信息 -->