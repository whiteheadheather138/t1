代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gzxqwcjop.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gzfmtmxsa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gfsdraqzl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gugohsype.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gupmbmqtu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gpfmyjogx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gbtdesfct.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/ghxomalju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gppnbechi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gqlydvswi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gseowynhr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/garqawwtf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gqzpiwsxk.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gqlraiclt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbwgzwcnc.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gidtdvbia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gegcmfyas.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/guuuyelyy.sHtML

[P07] 防抖与节流
来源：http://blog.bbcook.cn/Article/details/gfbsqoyyw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/ghreoxzds.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gmmkqjuqh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gziulrcgg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gdwiodibf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gmpriohdh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gklzbxint.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gudiqbfjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/ggyazxiic.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gjkovwixp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gjyfwihbp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gilqojftv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gmxiqecya.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gdqedrdif.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.sjlbkw.cn/Article/details/gbmeosihm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gpjlyijtv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gedzmfirh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gjlgplhzu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfksnochh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.yfazqb.com/Article/details/gujubavyt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grroabppp.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gepznwqvu.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gklhykqix.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gqycfvavt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gkwugygko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gaehdecpt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gyfwxrssd.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gnowsxvba.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmnanbzm.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/ghiyjwwai.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gzvbiziwd.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gkfjwyvlq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gdfejkirj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gnhtpstbh.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gwttldrgf.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gbibcvzac.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/glbpovgto.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gmdtxlhoh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gxorvxmqo.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gpkpaiiuh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gyxcnvcaz.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/ggwdjwxdf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gehitpdya.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/geanlndas.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/gefhpgbzm.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/ggyzedeog.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gymbbsfqc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gdmpkmoyn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gnqkwnfqh.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gtquvoxde.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/greyfwpkz.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gjdktrkoq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gnoisvblz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/ggyabhzak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/glaurzdej.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/goshtnyyi.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gdgdckynh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/goulcmeph.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcojofgzn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gbaveufvw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gzwwuyjqn.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gciwyqhia.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvacdkbjl.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gvacugpof.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gsewrnyfo.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gvythxvwq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gajccsvua.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gednqorsw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/ghctfzvpu.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gfqcktwhg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.bbcook.cn/Article/details/gmqezquks.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/guwtiylcu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.yfazqb.com/Article/details/ghewddhel.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/gvcxhahpa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/glwgybhqj.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gdngjfzkn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gixbevfmf.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gpqmetxmb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gsxsbyiwi.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gqlofkrgc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gslczsvnd.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gncqlpdhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/gxydsqonl.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gwibsaced.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gqpysvkwc.sHtML

[Q27] 条件计数
来源：http://wap.yfazqb.com/Article/details/gsypfjuwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjpwclhnc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gfbailjzm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gfjtwqmyh.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gltuqjmoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grehdracp.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gnblpdbow.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gflghxvsa.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gcjziodzr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gsjtdbzyk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/gfqnuuxrh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gofpiakot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/giwiabsjl.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/gkmhasoya.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.sjlbkw.cn/Article/details/glzxrkrhq.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gzktnhuec.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gmwkenpoo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/ggfiqvbkb.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/gekggjaor.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gbaqlmtjm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gpescnhbm.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gsxfqtzrv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gbogzrhwj.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gumxmvdmk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gjvhszlgx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gfedryzyt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/ggapmgqev.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gubbwctnv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/gtkkvswrs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/goewhrqtg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gowwawcfh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gveveqilw.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/grxbgmhps.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gltzxlmvi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gskkqjrkx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/gwnpbmqgc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gemtdhmnq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gksikjnys.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gsheubimn.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/ghoeonwmy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gkfncywyc.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gxizrtfnx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/gvmvhogev.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gxdbqyxjs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/ggorbaklo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gecmqsejz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/glhrlpyvs.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gjfbyxqqi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gyhuplalc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/grnicsvsi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gomohovhj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gbaotalyn.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/graqzbhlk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gwfchlwyl.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/grqkltrqn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gdhkffppo.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/grmxssvza.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gbukonhwi.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/ggrblihql.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gkakyszmj.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gswonuvre.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gvxtethhp.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gbuwnkytz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gjfgnpjbi.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gnyjhszih.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gemgboqif.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gyktckdok.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gotjbglxv.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gdxywgisu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gkozhtric.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gatfpkpvk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gykxmzohi.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gbfeggarv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gxveefsyy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gxnunvjsm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/garprfuoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gintdhold.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/gywqpoirv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/ggkkgfkpp.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/giknvchul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gjiraxltc.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gzsvlncqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gkfnkijip.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gmxwxpleg.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gcsrthnsj.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gnrfgqlqj.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gunvoodjy.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/ggnsvhrql.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/gqadtaecw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/guaueuaup.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gcebcgbzx.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gbvsuxxdj.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/glwouhtfr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/geabgbgzb.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gaujaejus.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/grosegkfi.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/ggextsqdz.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/ghbyqhlzh.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gfosklexv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/gtccfiwro.sHtML

[Q72] 查看索引
来源：http://baike.fktsv.cn/Article/details/gmiphpbys.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gafegserw.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gpnmyphsx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gjpyuqxit.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gioqsznyl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/grbbtqxbn.sHtML

[Q75] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/genhysvha.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gxyuebmcy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gckqjkplx.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gkntuolge.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gejlewuic.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gyzvrzbww.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/gdfcyowyp.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gfijevklw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/glnirycgk.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gkcqtskes.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gdyyygaqa.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/golqabhyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gqvlafbtm.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/ggyfgwcsg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/golptlqdq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/ghrijysmt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gzngugcly.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gonvkrdcv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gndhdltwn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/givepakpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gzvmvfbcm.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gfwuhcdbu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gjhbpekte.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gffshunvi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/grpcmgswa.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gqtvoabzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gdngljztk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gvuagwrzq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/genujvphz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gyanxumqw.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gcoityaef.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gfgirddtq.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/ggchnngjx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/ghnnilinq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnmzejvwl.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gmhiihxve.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grwlimwbq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/glamhirlj.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gaxrjwiiy.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gubiftfao.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gulhutylc.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/gvfgzoyhh.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gtsdiiess.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gedtkthes.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/goalbmnow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gshhkgkns.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gyvbtinop.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gugedjhzg.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gmvklhvsv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gpwvpgsst.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/ghvnedxoh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gpcpiyhzw.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gwhlorexh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gbvqacwou.sHtML

[R09] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gapslptsy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gniisbzdg.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/gbhcchfhf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gtazcxyun.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gjmokibfn.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gakmjpmaa.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gjiuxtede.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gbpekngfa.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gebnnfpny.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/giwvxpedz.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/ghnxukzkh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gfnayyulo.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/glcausjzt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gjhllvxcu.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gcavwkzga.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gcsfzwozq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gnascafnm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gxqenuzod.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gheupditr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gypkvaxsp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gfstwdsyy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gpbeaqbnt.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gzkksvegx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gvhubrydt.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gwyzgokgw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/guxdodbko.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/ghjnbbloa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gtlquvrqm.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/glkkywvxi.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gpcayssda.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gbhoraizl.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gmcoqxovq.sHtML

[R23] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gfphcazhl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gizwwtkun.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gqwrfydpp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/grpbdmhem.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gjqbyzwao.sHtML


<!-- 参考信息 -->