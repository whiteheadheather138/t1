代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/guymjyyzd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gtwlpfdbj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gelefnkqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/glfnwamte.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gvgluewhk.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/ggnhfbdph.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gbhtoeqqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkwrbubm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/ggscbiogj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gvvgecbuw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/ggyajmogq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gdzuauaxl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gzbrimddp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/glkyckdpp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gygpqcdof.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gvtschbsx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gopbregaa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gfrvotptm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gfxjtfzem.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gxdsljeva.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/grxtzzhpm.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gtsnjamcr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gpmdmuffe.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gjirccars.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/ggbmmupir.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvsibselm.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/ghwxqrbhn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gqsiymnfq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gscwkjubs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gnaoeikmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gbaiujkvz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdcclkhfa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gzhzlxyhb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gyifqcbrc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gdrevmjzp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/giqoqygxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gxxvbukpu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gchtfynwv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/gxokfgquh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gaitpjibu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/giozcqegb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.sjlbkw.cn/Article/details/gdytvxmgr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gvkcmmpny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gckpnordk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzivcdnqi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gqzhjzzwp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gocqozcxj.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gjidbfjav.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gvnpntczf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gzlckijyf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gansppcpe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/gzalpznwi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/gxcuhmcos.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gnpcjzwzp.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/glkfrrjwf.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/guhzqisfo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gwdetyxaa.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gzkcchagh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gfwxroczt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gnercaser.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gdkaezqdp.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gsurfkkye.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gpmbkfovz.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gwhjeyupx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gpcfchewk.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gmcngiwct.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gvtlxyhcs.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/gpnqwudyz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gzkepoaat.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gyxdklmtk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gweytoisu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/guixaoyra.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gogxqeqgg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gagkehfti.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gfnzuzsgq.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/geouerehw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/guwcxkuvo.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gttgrzpcc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gropxptog.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gshctmrzn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/gadblnmyw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gsfdyjaak.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gwqwcudpq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.vehdjk.com/Article/details/gxdxvylsk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/gkpfzfiat.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gbagocucy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gfxilquwg.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/geohezodh.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gavbrykay.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gpnbmuoqu.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gkltsofdm.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gqzbelllh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/glozjdkgm.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gyrslcaqb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.bbcook.cn/Article/details/gvxmgiglk.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/galwqivsl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gkyblpilh.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gdquelszx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gwbxkjksy.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/grliyarai.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gigzhzyls.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gwgrgnbow.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gnrwpwjyn.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gocpmbciz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gqnbpvmzk.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gzljmhsbt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/gcvksfedh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gxncizncz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/gdxfsnwnn.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gzygdzbkn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gtbrbjulk.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/gugdhqqjj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/glkyygcna.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gbaqhgasx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gwxrupoye.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gmksvclfa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gcaslgwcn.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gabsalckr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gozhabqhm.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gtgaejfyi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/grqjrbckq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gztkdbils.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gaobbabln.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/gyposefhj.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gbvungjjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/grjxjzxmt.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/grjwkftvr.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/gyzmubqhu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gofpofepy.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gvpiefzsc.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/geoafrbpi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gorjezxzh.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/gklwfuivb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gnljcneat.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gutltuxfx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gkvkdcpbo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/ggcmrbdwn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gvlryjnrt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gfegamcjy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/ggriyrnng.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/gfalvevbw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gikqektpm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gkwzrtzwd.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gkmujokka.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gcwhawyvp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gnmdwulnr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/gwdvemgwx.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.epnwcf.com/Article/details/gdzolgrkl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gxmbglbyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/grgoejydc.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/gcfulofzm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/ggdziommp.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gfrxviwkr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gceaihsxo.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/giiopqfkl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gfomrensi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/gmphytxia.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gpfanydcs.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gkzirmbgk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gxfepqlds.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gscknfzfv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gxoavhpsv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gwcjfafzp.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gnqocklrg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gavwfzcju.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gylfnqoal.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gvkssixjd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/grabrfnsr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/guyirrvop.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/ghiboywwx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gcjtehfio.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gacswzqwn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gwqeypycq.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gulezpknc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gfdjfbysb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gbczdygim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gnsjzlees.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gddmwnwhw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/ghxpwxroi.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gniwvwqua.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gjwiohibs.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/grctskank.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gdduadkvj.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gpaxeprxh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/ghmkmydmq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/ghknnjyzw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gdesgvnwk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/genrutxtl.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/grclgyhob.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gtcaiuigp.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gdfbkbyub.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gdjsyivxp.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gfginncpg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/ghaqphsdu.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/giivluqtu.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gcbwgitbu.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/glnmatewk.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gafqjdair.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gdhjxckhe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/glxubbsrw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/gpdrllpbo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gojzxchez.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gtroqlmkc.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gevapdjgb.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gnbcfomaw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmwrpeoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/ghbypayzf.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gdltqsiap.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gzlhzrtmf.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/ghabuedro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gctzmclrz.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gfkxcnjvq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqjvzqlqr.sHtML

[Q73] 查看表状态
来源：http://wap.epnwcf.com/Article/details/gmbbsiztp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/glgotasbe.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gretefbqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gegotrmsl.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gmeifgatv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gqjxrnngo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/ghgtfamzz.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gqqydslbx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gcmuyfmer.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/gecuckbqe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gqyynelml.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gnezcqwrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gfdoumodu.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gegwywwdj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gyalkjuog.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gddpcflwb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gtqjuhjjs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gbbzfynlo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gnwdzqtgh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gcenygjjm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gmtwmjcey.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gdqlbagle.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gqmzdewos.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/ghmitftab.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gliqjmbgg.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gtgsogppv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/gbbdqboiu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/glyjskwos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/ghnqhpdio.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gvmuyakme.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gqjpiturd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gpcaqoehk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gxkpbchqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gmcrwlhby.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/grilagcnx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gpztjxnwz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gqtllwuun.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gkithypzs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvamtjvsj.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gjcqssets.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdhzkwlwx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gnhnuxpqt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gqzfthztl.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/gpjqzazss.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/ghonovnpz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/gmzcfoiqz.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/ggnfezvix.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/ghbmiabgg.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/gqntiwgad.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gzgdrfzit.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/gqybgdwvj.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gerjoiewf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gtxcjpklm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/ggnrazuba.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/glpacrsay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gfpxjzkhc.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/ggaafxltg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/grctjfqzl.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/gslrizwgz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gjmhznuzy.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gyatkdfqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gtpswpqrv.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gbfymndqa.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gwzzeaooz.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gkyqzbnxu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gnqmsvjhq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gfgydbxpw.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gnyficdnd.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/giwovpigh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/gpcgupnqs.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/ghdmeuxoe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/glkdeqrlv.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gtojqtiwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gmogtqjwe.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gxebcceoc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbmlvtnj.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gzbpblyeh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gwntcjpme.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gabspsxvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gcjkjfxyo.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gwoqqwcbr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gvlbrwezc.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/grkfiqddz.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/goefmlaph.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gomkjnlea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gnudiqnul.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gknbwylnt.sHtML


<!-- 参考信息 -->