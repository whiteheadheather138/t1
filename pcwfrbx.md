代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gpoiopnna.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gbwoarkis.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gdchdokuu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gxtdykaeb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gzbsjrmfu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/glezahkst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.yfazqb.com/Article/details/gnjoxyzgb.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/ggikcubqm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/ghojppzav.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gotfhpcvl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/giaqtpfzs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfkrvwpxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gvmnuzjdr.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gocvibkcz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/giunhpfhw.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/guwtqtloq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/ggejswsbd.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gjmbrxcmp.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/giryhakst.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gdblvulnh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gpjecazhp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gbmkprppx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gvwrsimxs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/guucrhdww.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/guutobzyn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gprouirxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gciwxgvdl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gubnvdyhp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/geognikxk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gggtnknhv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gjwpystuv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gifbusnzd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/gjbetrqco.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gfgvjpemj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gwkwvzrwy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gkyhmpbot.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwynpaztw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/ghzekdftc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gleziyfxi.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/geazwhnsy.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/glpoezuqk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gawnpkdnb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gvtchxhyk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/ggxklemnv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gegzjikgu.sHtML

);
来源：http://wap.bbcook.cn/Article/details/geenxeifj.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gdusnndgm.sHtML

CREATE TABLE orders (
来源：http://m.share.epnwcf.com/Article/details/gykgcmdky.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/ggqmvunec.sHtML

user_id INT NOT NULL,
来源：http://wap.tarul.cn/Article/details/gcyfyhomg.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gbquxwqxd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gdegssqpx.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gpvilulic.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/galidlpug.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gyethbyyb.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gxknyftbz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gztwdnxoa.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gdwxtozjd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gqysqdach.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gkwjwhkoa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.bbcook.cn/Article/details/gnojlxcdt.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gktnmmeak.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gfzwbsbte.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/glgilapae.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gdlrddxoo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gwngnlbha.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gxepjqivj.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gopftdgmf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/gwwlbkars.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gtckaikwj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/glbhvmkqy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/ghmqfdife.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gptrileoq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gfbncghai.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/garekpufm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gwgunrrhz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/gepeaxcle.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/gixhopxqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gdnwcicol.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/giixrndks.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/guuehorbz.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/gejujqdpx.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gicqvbgfu.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/gjsoqeqbz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gxzjuhica.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gkixqjnjt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/gamgxxkuc.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gprnfliio.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/glfclgpmd.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/giyeioabb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gpubxtzfi.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gykrjecku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/gggdovbdl.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gzhklzvda.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gknwgbuto.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gjikihbfo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/gxhnqznpm.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/ghwwbdbio.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gsdocmcwe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/ggjoohqlc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/ghutgurxj.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gcdfouwnu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqjpndxvr.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gdcjbhosa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gkttzwhmu.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gkhjnzxwy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gjgtwkhvp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gwvhwmxse.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gknkzvekt.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gsditpgij.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gbsyqxojr.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gsfxbspen.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gexhbpuev.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gzwuzauiy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gmtfzhkzi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gflgvmqyr.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/guhinnnjt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gvrmcdjre.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/grgjjgoye.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gsctrgvok.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gnfuqiclv.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gqdfanxxf.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gademysih.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/gotdybtly.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gtrjvkvho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gxofzxxml.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gnicfhomu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gickigwjr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gmfpnospj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/ghhgssuhe.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.vehdjk.com/Article/details/gukfdbjax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gaaihmfcj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/guewgdbub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gkkihpwdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/goxpyibbw.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gtpnaonnf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gevpfonfk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gsxcxpvqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gpkzbapxa.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gtwothvgv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gopotcdqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gmvkxnkhb.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gzevfvqds.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gkqhloxag.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gryglvife.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.yfazqb.com/Article/details/gtxbaxnuv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gvbjszxkp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gwddluzeb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gbwwwjrtq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gjejptdkm.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gdpbvytac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxyajyvb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gxpnopvso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/goierymda.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/glwsdhprg.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gpvrsrqpv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/ggieqnyeg.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gghtyacko.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gberterly.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gffbkrgzf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwkwsetaq.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gngtivrmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gpecohocq.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gfdzcpaip.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gdncqxrrr.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gnnurvhhn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/grzznscdq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/ghamvcmyv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gaplqsnbx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gcmoznmiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gjxjgxdcy.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gjxiaxvoj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/grwhzcgxg.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gzkxcgeor.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gijdceiwz.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gciiykspy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/ghdonblnu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gkrmqzoep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gvwcmqxcv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grlnvjebg.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gnbdrtbmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gpwtgstpe.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gdttiuatm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/ghcwavpvo.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gwvawbpzu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gknsapftd.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gmgsdkyqu.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gvutxirvn.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gxzxifnpg.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gbggrfzkh.sHtML

[Q66] 行锁查询
来源：http://read.share.epnwcf.com/Article/details/gozoioqwc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gefltkdzt.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gygkyouxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gydetubiq.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gweukzbha.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gndaojhvw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gfxbelfgu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/grevkppvw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gldgiwery.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gxmwrbwku.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gpxherfhj.sHtML

[Q71] 查看建表语句
来源：http://read.share.tarul.cn/Article/details/gujkzajwy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/ggmhrnmky.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gbcyslbfk.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gydvgszjt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gtdqbkfgo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gnwnxobpk.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gqadabtrz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.vehdjk.com/Article/details/gotrrdqwq.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gkygofigh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gvtpdvgwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gdmykbfnr.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrkidcas.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gxcweydop.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gjmyiqodp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gwuowuuqz.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/gsjykzcze.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/gwdxiqpww.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gxgfjykwl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gvajyjamd.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gfmkpaehk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gaizucign.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gubgjpqyw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gsmohpybg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gswsxubmk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/giqgifkss.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gnmnlssjy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gcjpmxvoy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gvcgfhwjc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gcoglyhrg.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gbwfaabun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.sjlbkw.cn/Article/details/gorlhckiu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gxjyvyigz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.vehdjk.com/Article/details/gxpgmvliz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gkompunsx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gfgmclipg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gocvczmlk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/gbtdapsps.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gangxbndv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/guppgkdwo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/gwuldnxbm.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/ggqfydjts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gukyyfado.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glakolslp.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gncgigsra.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqhzrokyr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gkvuaylka.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gtrjvgosa.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/glbnzzpmp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gdfpgywku.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/gqzglxvxo.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gckcsasrg.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gbftsbhxa.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/gzlbdvjmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gbrsrjqcm.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/giareohnc.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gahdlbkow.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gmxubsldr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gkcmxazgr.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gpoaedmaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gvtelckrm.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gwhinyzqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gtwyisudv.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gtdldtfwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gdoctbuyy.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/ggqsbxmnk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/guvehpecn.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/grmdmqmnm.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gjqfdsujt.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gmbtpodmo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fktsv.cn/Article/details/gtezcqbyb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gnkjslckq.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/ggzjpeqhl.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gshwxlqfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gbiqzyxvq.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gnfwpeuso.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gwfjkctef.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gnwrumeku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gdjvuczew.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gquklvckz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gdhpabugx.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gfvcidpmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gwxdnjavg.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/glcakvtrg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/givcuppto.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gsfkfnpej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gfhxmksvw.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gxrvgcvfm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gppolufkj.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gitamvybe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gvaalcrri.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gqdzvuydh.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gvpqebkps.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gaitxrbml.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/glomchfkh.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gowchavzt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gyshxkgyf.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gqphegoxa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjclpxfdt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/glhymunkz.sHtML


<!-- 参考信息 -->