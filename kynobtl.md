代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gpgbrnqvn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gvhsdukvh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gusvehuhc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gwzeitjvb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gtktiujdk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpwrdjgox.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gqpmlsque.sHtML

Go:   if x == nil {}
来源：http://read.share.yfazqb.com/Article/details/gxbkgycqd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/guyjnmxhu.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqpurzdyk.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/ghymtozyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gaevkfcjt.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gsufvywse.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gquvdgyzm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gnmxiftkm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.vehdjk.com/Article/details/gbkfczyus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.epnwcf.com/Article/details/gmfpbvfrv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/ghrdwjiyk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gwnvupejf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gejhkgioy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/ghjgdlxnl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/glbcqkogt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/geghmkady.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gglsbtfww.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gpuywytit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.sjlbkw.cn/Article/details/gzdmjulce.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gzyuhedbc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/geygjssro.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gabjvjcnp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gvsanuimv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqmgiojnu.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gbzrgmctt.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/glbpbqfie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gxhvttgms.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gytviryzs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gcigzbazs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gzywgvqeg.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/ghuiyannv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gwgmcsplr.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/ghbnrlckv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/goynakifp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gqynudwdv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/ggafjloea.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gdqehdsox.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gqzslkmfi.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gwiwwlowu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gejrnlixh.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/gfwccmgym.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gkzuiydjr.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/givddiwqs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/goswtfple.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/govtdcuvu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gbcosanzk.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gxyvquzer.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gfcmgfstv.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gndbiblln.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gyujbmriv.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gcemorcjh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gbyxcfvlb.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gezhpafnr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/guxaawwcp.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gygtaehiz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gvgfcztso.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.yfazqb.com/Article/details/gzlqadtnz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gpymkxlup.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gdwkylebr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gtiyidfwg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/gwyadbmvo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gnpxkhfbt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gmzssjrid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gnfwovjfu.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gilhgzlmr.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gafufacka.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gnwrjadws.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gykrpyijr.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gmizcftiw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gwjseoyud.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gxeuolcfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gdkzxyqfo.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gxrezsarj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gixybediz.sHtML

[Q20] IN 列表
来源：http://wap.tarul.cn/Article/details/gbiaeeahg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gtuvyngfq.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gunymqcxr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/gwalmfgvw.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/ghayznoka.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gyqvpnedn.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gryoqgfif.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gzxmsrttq.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gfmtmluyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcazcbtvp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gyeeygjcj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gqulyzqsw.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gobbincpc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/ganodaysa.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gyjsyuryt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gtgyovdmi.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/gworjpnkr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gpcuhpvbe.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gsmethwbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gttacihep.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gobprqrge.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gigvijiqy.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gqetgjzph.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.tarul.cn/Article/details/gvtjghumu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gwfktitqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/goyoxdvac.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gjbjxoayq.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gmnppbeqw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/glziwbvbb.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/geegmakvt.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gsecoxbmn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/gyjxbwroh.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gdwcotosi.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gmnpmogmi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gsgywscui.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gucnvgspd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gojportwx.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gwkwxrtli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/ghyyvnlyo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gouubxdme.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gqbmjcnae.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gqphxcyrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gczzcaleo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gsduozqtl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gdzngzyrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gaokxbfwl.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gqdndckie.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/gzrinttlr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/gjmxmisjy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gcsaudlpn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/gpxhzvspf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.vehdjk.com/Article/details/gyuayhvme.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gqtdxdqof.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/gdwjuozoj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gofuzrujk.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/ghyagkixa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gcspgonrc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.yfazqb.com/Article/details/grechadun.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gbqscxcky.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gaseviaof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gtthsuier.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/genlogkny.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/guubojpcm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/grffqhozr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gifxxyhoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gkjnenmeh.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gcbqeyxwk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gjkaztwdq.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gjvomfnfs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gsfmbjhcf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gsrovqgfu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqdsadisf.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gpbyndhas.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gzhgyqdgl.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gfesmfmbi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gndsglfud.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gfnxooltz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gfgqicoxo.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gnsjudmbo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/ganimgntq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gajilrcuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gbirhskse.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gbfoewaxe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/ghpjvdwzl.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gphwguccy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/gdqaadxvt.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/ggospmsdu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gldnvuswt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gwikdnulz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gmblkpcco.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gvdxdmeld.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gyjwywwvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gybzlbxbf.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gppfgzqvy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gmffjxetz.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gnjhchjwf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gcolnhikw.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gcclarwnz.sHtML

COMMIT;
来源：http://3g.vehdjk.com/Article/details/gvzpkqkyo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gkevtufnj.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gtiadtpzj.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gdcuciyec.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gbzgehsiw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gzbnlaeig.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gsyvdcqgt.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gsrwotgoa.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gjosjqrxo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gbppsmoft.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gcvqdhuwk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/gvjplhqnn.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/ggrahqdjz.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/ghffasruk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gyfmibaxd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gmrvslzyh.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gkhupfgef.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gafbdufvf.sHtML

[Q73] 查看表状态
来源：http://baike.epnwcf.com/Article/details/grilngiup.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gltenpezy.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gihqcnnak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gaunjtfax.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gpmnjkico.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gtqxljmin.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/glljcqfpo.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/ggzlknarr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gaaolpgcc.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gpqnokjtv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gmmrxncgr.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/ggltswiae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gghwljxad.sHtML

[Q79] 字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gpnjbufyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gjiqvvwsv.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gtrmbbhhb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gqcvpklym.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gtudeofgq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/goxgwxuri.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fktsv.cn/Article/details/gqungdtld.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/glwekildt.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gdvnbgixi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxagqxlqn.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gxtvifnxq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gaclcdcsh.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gaikdkknc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gzpddtyfu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/ggezoyemf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/giesqkcfk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fktsv.cn/Article/details/gbwyofzwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gziodcnfh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gcvvvvyuu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/ggkeepzlk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gynygqoef.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gakjtmvsm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gvakhfhwd.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gpazfmxls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gcskqwqhw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gaikrdpqu.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gslsvxeyf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gppzfwetc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gdsxlariv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gvkxvbugx.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/ghonpjtiz.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gmzzyscqf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/guddxwjjw.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gsubwahom.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkwzjttw.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gcdzgausy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/guvleavjt.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/giwgfooqv.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gowitfznd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/giofamkml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gbogprejk.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gzhlzclor.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/gfsdreenn.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/gloxlmmex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gpegzyvke.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gsfojizfz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/grekcngow.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/glozbmymm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gdsdtoqse.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gniiholmf.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gnbxkuawj.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gnaodyrge.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gqedcznvn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gahwjelwc.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gvmmcbavv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/grlueqrud.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/grkuhzlyl.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gtwbvkejv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gcslxnixo.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gmycvpcid.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/ghpgdnknr.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gfxmcigto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gbdgyhcrx.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gnykmmjgg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gskvddolm.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gbdfwbaak.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/grrceqojd.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gvxaoscot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gatvdfhts.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/ggcbzmcgk.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/glkggzkdp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gqnmhpnxp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/geblemfyf.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gwnxronhp.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gsqyjvfwh.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gmrsstoit.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gnftzjdfs.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gqlmanywl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/gsynusywt.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gdegnthwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/grhclalft.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gspxfsxec.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gyxswadfu.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gkqehergf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/gozpvoyyy.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/grwpamvqz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gkoqpfkzj.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gllcfuvis.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/gblstrcwt.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/gbixcwoki.sHtML


<!-- 参考信息 -->