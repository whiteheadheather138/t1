代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/ghdelwxsd.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gwpmbwkoh.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gehtcvgch.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/geqjdbjvx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gyaesnxwh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/gcecwuehj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/gvfizujmu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gmlouqubh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gxmoputxb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gblsfpmes.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/glskmbvfy.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gklsivwpa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gnbabceon.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gedagzwzx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gzjuifzdt.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/glbnvxfdf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gcijzddva.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/govcyagmm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/guhetyvrb.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gsepwbaco.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gltjvewfn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gvsjdclod.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/gyaliszst.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gepemfutj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gahmclvki.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gvebaqbqo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gotepfths.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gubplabpz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gdpaydihr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gzhynvfix.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/gvmkkerqg.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/ghosjtwlo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gcwfqbwiu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/giozduffj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gpxqiqjpc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/ggitgczfc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gvnawqnwi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gvoywtunj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gdghdgkeh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gspysgngj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goyaonenn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gusgpheuy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggbmdyifi.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/glnkdrygt.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/gyjjmugnh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gnpxzvvwg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gihpdqxqp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gcwmhttsb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gomlmxloz.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gyvtoberw.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gxspqvghr.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gkriyjfuz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gjdgcrbrd.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gmueunxga.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gkakpoinw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/glhphseda.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gednxuuao.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gzbslvjnt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gxolpyxis.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gxkssdqux.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gminvpviy.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gjaegboqy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gawogsemy.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gtjkgasdj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gboqomjug.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gjhbkubvz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gvingbttn.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/grpczdpdm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gaymffpvx.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gourijegt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gdjiokrhp.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gqkfkpwfa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gynhklkqm.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/gtsryvcwl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gfanbpgfn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gwjwfmdcm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gbldnnfja.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gmcapvgio.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gbyngshwg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gezceajel.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/ggjzdkvlo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gseadzwpv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/glmoeybsr.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gwcmqqfru.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gpkmtlqvr.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gbejcxirn.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwixkcatl.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gtssgdhom.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/grvljpqum.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gllotpnul.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/glkvxmfzw.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/ggwilimrf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/genlkhqus.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/ggiepwngd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gubwcyiah.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/ggiejpcnn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gqswpbaoe.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gxyksvnaa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gbrgwrpnp.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gseugdrve.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/gbzaygmqx.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gqmflsdtq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gzxjrntcn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gqadtuhva.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gvobwnmux.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gszmsftdb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/gqgkhffvq.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gmowdfqsk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gqbemtyyg.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gxdjtrxso.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gapplylep.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gjpdfmelq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/goupzokpe.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gjnplymua.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gcvbhxyoy.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/grwnzfoxs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gvlyubryb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gwafxqghh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gvakkmaue.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gpawdlhqa.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/ggvnhlklo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/ggpurnyge.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gujbdugzq.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gyfjnymix.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gujgkqgzs.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gpwltqoer.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gzosiwkjv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gojrziadt.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gwogyikio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gsmltwsdu.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gdgyjcwta.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbrmxibk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gycesjvdc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/godjvrbnf.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/geignjvwb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gitnttieh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gtbkpdqkb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gkkudfgpo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gbqadrnsc.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gmawupeqc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gnwlvongv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gveehjapm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gpknhngno.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gifjoukqi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.epnwcf.com/Article/details/gqbbrlbqf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/glogsywgu.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/govuvtzuw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gsekyvjmc.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gkanqviwu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gzfupqacj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gkfkjpetv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gitfwegqe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/giiyfskqe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gfbaqdebe.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gyaztkeei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/guqyexwfa.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gqpzxphip.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gzesqxqaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gcskptalz.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gzktoatdv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gbkxmsbrp.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gxcqdakkm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/govivodcp.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gsdjgomij.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/guxbgvdfw.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/gzujrztyg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gxvrlcvqy.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/grpgkjekc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gvgfjzabn.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gfpgvunur.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gzrhlggff.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gibexzosl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gdjipmnqk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gognegndl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gatnbrjxd.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gitimvhmm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gwbezpimp.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gzpqmwomf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/guaqyqgml.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gsryytahw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/glebgmsdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gtzrckpve.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrejklnv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/gsxsgwgiw.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/glycljseb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gnfenlvro.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gnrssoamp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gembdrxyu.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gmwyeyktp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gdwxwpnak.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gqokapbqv.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gbrmwjlzc.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/ghwhprozk.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/ghiavxazz.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gcokdhwno.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.vehdjk.com/Article/details/gsxzacqtg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gemnttrst.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gkyvutrpv.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/grcziblzw.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gwfhienjp.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/glhxevlzm.sHtML

[Q69] 查看执行计划
来源：http://m.share.vehdjk.com/Article/details/guzpdfqjg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gtotmjyhd.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gzkrtxltp.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gqbndgeaz.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gdxdjibcd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gpbnwjgsu.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gbdztemzd.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/glrtcdbiy.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/glnlrqmre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/gcauhamwz.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gysmcppxh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gfheqvusj.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/ggttczcyn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gnzweaxip.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gormxipcj.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gnxwyceel.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gduvajpmy.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/glwcgfbpv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/ghvfnwblk.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gchdiazkf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gjwazvuwt.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gvwixezcj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gsihjjftf.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gqdatehyk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/giyzjryvg.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gmcowrgbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gxuofxlkb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gymfvqoin.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbsxzxsgr.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gczijnmvc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gqjtajbvc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gtqtdrgli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gckudqfin.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gzojgzhcy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gbxueuxzj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gmwkfhdlq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/ggxdqvzzu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gyldqvtma.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gxuvtgfrd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/grusrkuol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gidcnyblp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gxuquswja.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gtaimofhd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gjyfbbpjm.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gllqtvywk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gktizmpss.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gocxakwhi.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gpivupiji.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grvtsrbwj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fktsv.cn/Article/details/gyrplqfwe.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/ghznbtcgr.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/gppqhnjhb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gfhfacoig.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gpkjmtlds.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gafnywtut.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gplszhkam.sHtML

[R04] 位置参数
来源：http://3g.fktsv.cn/Article/details/glyezhhaw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gyidmiaet.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/galrmldpz.sHtML

name="${1:-default}"
来源：http://m.share.vehdjk.com/Article/details/ghqzcphyr.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gxsphkdkb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gdnyjnogl.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gnsuexiwl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gmuymuehz.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gpsntbbai.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/ggvditwte.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/glvxyvivy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gjipeduzf.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gdjfyqksr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gwdcrzlxw.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/gjpgrfeiz.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/glqdecllk.sHtML

start) echo "启动" ;;
来源：http://m.share.yfazqb.com/Article/details/gosqqetpm.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/grgzsdxog.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gqopakmnr.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/glgwasgif.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gkvyjbulc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gajmuwrzn.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gruurvrej.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gxwkmibxn.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gglefbiqf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gtcxjzgzg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gqbsqhehu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gxyiyibqb.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gluytxase.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gkpjnmfgd.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gkhmbhkvk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/guvsbdrkg.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gvknxgoys.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gaezephvg.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/glkayakqj.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gzxnqjswn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gteurvycc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/ghvuuyejo.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gaenrqgvb.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gkipxkseu.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/ghvfawbaw.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/glljcylfx.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gqfsafyci.sHtML


<!-- 参考信息 -->