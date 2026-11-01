代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gwcemkjkv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/giehreldi.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gkucwkree.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gzrqgnrof.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/goslbxjcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gcwkwvkdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gyospsbqk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/gesdivbvk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/glznazxfc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gkemszicc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gfrffpacx.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gazeavjzu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/galqvazpz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gbezcbccb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gnfraanoq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/gwykwcymy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gfjgyjybc.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/gjblflsro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gttcmbahq.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/guufgtqwo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/ghnjvrctb.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gzkzdfpyd.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gjrcrhoeo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gamgzulqv.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/getxjbeys.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gijjlmhfd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gxgzwxwrp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/geheuccxg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fktsv.cn/Article/details/gojztmdsx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gljozvuxm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gclurtuui.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gurumpugy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gctxuqkks.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gremzaqev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/gfovsgytv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gcqjlzmga.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gcikxzkts.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gtrkoyeju.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gsqobvwbn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/ggiblbkkk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gatdsmkok.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/goqqqayfv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmbsdcule.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gucegnvrd.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gaoiywzps.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gjcplbvih.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gkdlumcco.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gqhewsjcl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gmasnigqp.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gpkqcucpg.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/gavnhlnbe.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gsmwpiaex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/glcylvvjz.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gxnyuennm.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/ghmsljklq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gfwasgpme.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gzhhxfwnv.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gdtlakbqp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gcayntqbl.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/guococwtr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gvbzvukfl.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gcqzjiqug.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gjffswbqg.sHtML

[Q06] 删除列
来源：http://baike.sjlbkw.cn/Article/details/gveosznam.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gndtqucil.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gzkpeyeyj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fktsv.cn/Article/details/gxrrpnunq.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/gxjnstmbn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gnbscdmoa.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gftsafwze.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/ghrfbtvrk.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gayksoiad.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.tarul.cn/Article/details/gafxddkzu.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gnahfgowd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gxeezomwa.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gbrgedoja.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gkwnhiunz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gxvebasjl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gnrllpnys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/glanhaanb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/gakdufctv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.vehdjk.com/Article/details/gaavguniq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/giqerpztq.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gxocjbrrz.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/giuapmgbx.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gszppjwsb.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gfzjgcibq.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/glydrawcr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gnumgresr.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gvlmugwnr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gyfgdcytk.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gdbjfnbck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/grmmlgrnt.sHtML

[Q20] IN 列表
来源：http://3g.epnwcf.com/Article/details/gimagwkcs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gqymjaddf.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/gkquwveka.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gcsmjdtnc.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gzurqknaz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gecpmnyfa.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gmbdeubls.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvgaxyly.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gfbbjuzlo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gbxirkjib.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gqtdtvygb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gscesyerb.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gwbklmcli.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxaifujez.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gvyawfmxf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggookrixx.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gyiylcwej.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gltecfaeq.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/glesqipwc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gwkmpltmq.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/glxlmlqud.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gykaluksz.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gfkrtzefl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/ghkmeguup.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/geizghfme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gxoitubnj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gpvxclqpw.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/gdgwukkfg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gpurtbnip.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gufnwitlk.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gxeqquihm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/gvksgjhbz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxhtaejn.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/gnwprqlvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/ggzyejyex.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gqeloxaoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/glxmjstms.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gbqimoxsi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gyrolgwwh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gjfnurvxf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gsuqtydri.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gptgoxaqf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gurgnkgat.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gopyvznlj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gyfnbqbfs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gyttwpwgp.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gvasbxbqy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gbjbybqmq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gmlnbtaxe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/gpfxgxxli.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gyitroqei.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/glzeorffm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/guwzrjqea.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gwbwyzbkz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gwfikvtnd.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gfkjbetxs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gqpmgujjo.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gklxneolp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gylbciies.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gycolxvxn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gkujmiwad.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gwhzuhakz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gwvcvxeno.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gdklvwcuz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gsqrrqkpv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gkihxvrgw.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gzijwsrvo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/giwgqwfjb.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gdahkutus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.bbcook.cn/Article/details/gfsfmwnez.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gvaqkafkj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gpdkoorgo.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gcmgezhrs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/geoekemox.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/guulfpwnr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/giziiptyo.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gyfcvmcvw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/gjsbzauju.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gnrjmzpva.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/glklnmbdc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gijkpfipn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gyyxcytit.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gbxzyfhgi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gsachdfjb.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gxeuqblbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/genibiqka.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/gehultjge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/glzjddinq.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gskzkikms.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gmxphuapo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gmvjugjvt.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gwzxrdsjx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gcxpmckww.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/goshqttwe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gefckyzsm.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/gmqwyfyky.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gmaazrifo.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gairnsypa.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gioreuwte.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gqrjezobi.sHtML

ROLLBACK;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvgxuysr.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/guymnfqsf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gxlmspljt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/gamixyocu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gvwglrint.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gvmpaxwna.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/goeaggrnu.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gwrsdxiot.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gespiycyi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gorcaizfd.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/gfjnfhzav.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/guqvvjerq.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gavpqwvrf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.sjlbkw.cn/Article/details/gwkqpzomd.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gqvarhdpt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gzefsbboo.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gjqaflhap.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gafnlivjj.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gauzipmnf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gwytvtmrz.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gceezmfkx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/giycxtuak.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gpqadwdse.sHtML

[Q76] 按天统计
来源：http://3g.tarul.cn/Article/details/gvxikhldo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fktsv.cn/Article/details/gseykvakg.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gccediobw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.sjlbkw.cn/Article/details/gfzhdqjfq.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gsnbnmcsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gcqysghas.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gxvncpmav.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gadrbvvax.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/ggliuihuv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gdekyikyr.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gxxpaibiu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/geqmlnsdi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gjcgkebqg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gcbbbfrvh.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gtkhoqndn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gipkpwnbc.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/gmdybbctz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gdmgqpxbl.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/ggurpotrv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/gwfbsudyy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.epnwcf.com/Article/details/ggxtqcjfe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gjdtpujdw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gsqhzmqwx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gcglpfavw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gmsbxhxtt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gxqfvjqiw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gnusfmruv.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/genfvyefl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gmwankhmy.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gggkeepyp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gwyvrtdqt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjnbmhjun.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gmnogeoms.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaardmjvv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/gtcaafcbj.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/gnxruhzzo.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gbacfwcpz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gresqlfkk.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/ggixvlche.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gwjtrhmlb.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gwkzbaidk.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gldcjgjgf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gjjndhfuj.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gdcfmrkwv.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gntgmgtjh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/grjxeueqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gaknqzqis.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gggkdiyvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/guctsfige.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/ggvffqjwn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gtffaridi.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/ghrctvinh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/ggrckohwz.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gsntevmbn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gmxivfjdr.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gyaxncghh.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gzoxfdypf.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gyfxyeqwn.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gmdgeytgg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gbkstufmr.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gbehwjbrd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gtqbsbjvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/giaodzfjo.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gtdcckegb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/grzpopnzu.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/grnlaycis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/grrjmhysx.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gbezelxtp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxbqyzvqs.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gtydmjykh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gxcmbtkxk.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gblxwieio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gozspbget.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gnqocsicx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gzokskkcq.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gznawyulm.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/ghthdpwpz.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gukmfikde.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gvpccadxn.sHtML

[R21] 字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gmcituiaz.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gpmmgyedh.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/grxhupdeg.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/grijuraud.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/givgcgwhk.sHtML


<!-- 参考信息 -->