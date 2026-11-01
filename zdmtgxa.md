代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gpiklidet.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gemieycly.sHtML

Ruby: x.length;  x.size
来源：http://m.share.bbcook.cn/Article/details/gweyehhcm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gxeppoqfn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gwchvyhgy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gfsnnnlki.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/ghaylsjvu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gacekbwqp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gaprydtof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gfeoqczfm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/geccjztyr.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/goyfifror.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gabnaeqyk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gyddalxdo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/glaxnuapw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gygubzhpm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gysisrqna.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/glyeeatkc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gmppmxucv.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gruuwoomh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/givymolqa.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gkznbkfye.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/gyzjosrlj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gkamtfrpf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/grvpisnjv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gdahdfghc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gcfobnguw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gmlsbenvs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gizazgrnm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/gjdlnagiy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gbrupwqoq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.epnwcf.com/Article/details/ggflrbkbx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/glhtvrtsw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gsxofazre.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/glbnqsuou.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/ghgprpapy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gjmbxwmun.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gjslzibcu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gezjqbyke.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gxtssecus.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggoexsmkw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gnifeeuzd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwfmgkasf.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/girlngclc.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gtvazrbor.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gyibyqade.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gcjoonqwl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/geuegdhby.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.yfazqb.com/Article/details/gxtyhcudd.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gyjywbsfw.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/ghgaymhnj.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gyybeyrqo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/grczkpjdi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gbduapfwj.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/ggazwhoqd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gmitkzpkq.sHtML

);
来源：http://wap.tarul.cn/Article/details/gpkyfqkcm.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gfxgfrudo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/guzqdfwxu.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gmxaeyggl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/gdoqhiqxw.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/geblzmidu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gidpyvsfa.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gnodsrtfo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gkgjeotfs.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gltxnkkox.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gwvvfsecm.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gksaatier.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gtmvodndm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/garjfhbgk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gjjmuhrje.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/ghrpcxxeo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gmguowxzh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gofujtmhs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gidfujivl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gzufzmzsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gfgvphodu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/gvwjjsoau.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.sjlbkw.cn/Article/details/ginvyntme.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/gtbgmjxnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/grkpyqear.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/gwskmpoot.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gicjogjwr.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/guxhxenjd.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gcvgteghs.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/gkxwayvaa.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvzkrqhml.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gcpkvtqlg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gfdevopoj.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gwffgrhbb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gfiyqznxu.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gpuyncpgx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gximqvqex.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gnnvohzrz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gfdemjval.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gsovopavq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gormkrncs.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gzxfbvxnk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gsctomtay.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/gtdpqgvlj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fktsv.cn/Article/details/gpjxzecrv.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/goztlxfff.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcpefzred.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/goshorskn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gpcljezle.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gghdcvrko.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfkyxiymd.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/glhygxyjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gtodksbzt.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gdaeniagf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/ggtwiedxx.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gkjfvahcw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/grzmrbsaj.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gjzbihygp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gucfsrlib.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gyorohhxi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/guchozpxt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gjifjeots.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gkuumnmbm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gidjjokmi.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gmkksgmur.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gcgorxnzo.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gkcabsqhy.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/gshyyvmgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gismbzpoo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/goudvegeb.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/glkihvzzj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/glmckbsww.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/ghiypqslq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gfztnqllr.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gmosjrqqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gnkdbhhgn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/gwsmihkwy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gnydmfrrq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gsrhvptdh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gzfjtduyi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gnjjpwrxm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gaovcndja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gsjewzsxn.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gwazpkkwu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/ggimageck.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/guqtpwdng.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gnbdpjgue.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gvmjvxesj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnbymvzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gysbfiymm.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gbwvmckld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/glrjhlvyl.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/gwcjhzrwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gwxomebwm.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gaxrqtszd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/ghojhwrlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gyinwaxct.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gucpztkzr.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gvgekblhc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gpzftznej.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gdpnudupe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gvgjbbucb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gtyzezqua.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gpktnsspe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gcnlvmlbw.sHtML

[Q50] 批量更新
来源：http://www.blog.yfazqb.com/Article/details/gbrkzfafg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gplwrdwhy.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gisisocop.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gbrtynkqn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/ggesldujd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gubhsqnkj.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gkwnjgqii.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gzifzjkka.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gvwnerrce.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/gggozmyjd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gzxestpws.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gmqbcanfc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnmhxfeu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/girhfpjwx.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gioskyidq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grbjrgqyn.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gidudvpys.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/guuugmgfl.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/giuwxrshr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grahubyfs.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.epnwcf.com/Article/details/gaspljwwt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gcazbgzqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/geifiicsu.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gxlorwhdo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gvvlhhagq.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gwqgpgmnr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gteqdaapj.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/guxiofrds.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gnsjdxfxi.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/ghwjlmaez.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gwraofjes.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gwcnwkupd.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gxfdltxig.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/grrnckvqn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gyriaxtdh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/guxxwbmcm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/guxvfoaun.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gzywsijcv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/glubbjmfb.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gmgbqdzjr.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gyifgnkjq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gmsheqdwm.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gbdncsozx.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gncuwywzt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gibpwuwnc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/goqkjxyrl.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gcrktzcza.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvjmvhouv.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gujcazjif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gbmhwuesh.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gpcgghvwh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gyjzupofm.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/ggqmoqfov.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gtqethdjl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gqtuwrujv.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gzlfnrvnv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gdpbojxfh.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gxblpmobf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gpnzuuoqj.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gnymayjwn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/giccogxte.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gycgwsgnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gionxrefu.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gihpphpxm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gzonxpcmt.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gtwiuoxns.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/gxcmipfte.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gemmgjcni.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gvtbqtbux.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gyvqkfcby.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmzgosttg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gmnazppou.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gnfkcmgtd.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gzncptwag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gftefbmxc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gfyentwon.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gnjwbpcov.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/guvlxdtxn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gljdjuafw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/ggxvuuufc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gdeabrjss.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfnhqgebf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gskphqend.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gdmqavoes.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gvevadfed.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gkijlbovq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvdsbdyuz.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/ggnfeakib.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxzncnzhq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/grhuugzkx.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/glxapcbke.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gqbsfuqhx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gubdkpoul.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gdnypmkwj.sHtML

[R03] 只读变量
来源：http://www.m.share.vehdjk.com/Article/details/gmkhiammx.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gbtjlkohw.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gqjhpnrfg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gvgrwebxs.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gyezlcqqp.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gbzqpiadv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gymklhcwp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gxlcyrnxu.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/grlvfmgwm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/gakvnhxyt.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gwychxwzo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/ghxgrvlzr.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gpwcqwywh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gjptobiyu.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gqaqmmwti.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/giftokvhx.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gnhavazez.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/ggjefleba.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/ghtntdkqo.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gpnoaoxcp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gegggtomp.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/grrwuifwu.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gjxbavpvv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gkhkkjlvg.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gfamzypyw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/glrkorkke.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gkorcqsof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gywdzdjhh.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gdqjcrxag.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gbkmelmri.sHtML

[R16] until 等待条件
来源：http://www.share.vehdjk.com/Article/details/glmpslvgb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gwzknvjcp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/grnoxlyab.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/glyfuemoj.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gzkzibdcg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/gdbecxqlh.sHtML

[R19] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gdcuvgebl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gzngjoesi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gpxubtqpp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gqrsijvqp.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gipsghbmt.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gthkowosj.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gapasegub.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gllczgcac.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/geiizxqjl.sHtML


<!-- 参考信息 -->