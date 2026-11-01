代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gfjtsgipe.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gzrvnpvvf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gymtktxmr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gbhzvojtr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gueurdmyb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gxkeujmiz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gtigghvnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gwtabwkoi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gffcbuzju.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gnbgdpnwe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gkisqkbpz.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/gsnzbnbqi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/ggfjneahm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/goebeekyj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gkndgaweh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/ggfdlgmhx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gahdzlxcp.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/giopvqapp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gldoddrez.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gvfywaspd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/guiwcvoln.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/grdjwkokm.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gteehrapa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gdbzphrtm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gyongbzme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/ggjsmiuri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gixkxagcn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/glbralzjq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gedcjmqrr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gjbylnork.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/goynekwxq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gmibasyii.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/grixwxcgp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/ggfnanhuj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gdlnztrfd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gfdxvrqbb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gpqsryvzv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.yfazqb.com/Article/details/gpybqayun.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gmcwurwld.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/ggfgqzfzo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghmuiorrz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gjdwcfvct.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzrfsojjm.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/gedfihosx.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gvkffperd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gwfcndncm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gnlplsmof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/glhyrvjhs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/geueichdc.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gfkqnztcw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gcmtibfil.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gdskjfeob.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gkxwwvqag.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/ggvdekayo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpwhooee.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gtkogtyli.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gdmtwlcgy.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gvwhblxxf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gcldtjtnd.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/grhcmelog.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gwvjvwugn.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/gqnpsilxy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/ggsihhobk.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gjwefsdbw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gjdqezzea.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/guhsuleus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/ghpdbpnwe.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gdouwvnhi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gnoufvvsh.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gruitvnbk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/guapgucwq.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gpxztvlax.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gtiounirn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gdqlcmboe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gsaxknarg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/gbrpxrqwv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gdmkjxxgh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gzojuvphx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gvbojquwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gtzwceobe.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gbjrskaot.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/gcjebtuic.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gzcrhqfwm.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gmpblyjzr.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gnzqikuwr.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gmjpkqtmg.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwxmmyftr.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gqxbzpors.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gwjulifwx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gqgodwiyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.bbcook.cn/Article/details/gvzxvrkaf.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gkftqiuct.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gaemhsluk.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gvtbwweqs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gxnlrbcgd.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/gmdqgwvwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/ggktjpuqm.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gzubuxtat.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gqgqqlllj.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gckulnjnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/ghpzbivls.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gtzjdfppb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gkmysdavz.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gmivshamm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gwjgesfdv.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gcevtcoss.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/gjulhzfby.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gbdbiwfkg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gumtlubpu.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gpnzgkkvq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gatbeewfu.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/grjrvqtwb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gigxotusa.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/ghkpgfvrj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gkdaoskdh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.vehdjk.com/Article/details/goksqqfnx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gakagigtd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/giqfecifc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gfbhskrfk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gtrtekxgf.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/glnjnzjhy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/gippsnbli.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gqxgndjvk.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/ggbgsghyb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gnzqrlanr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gglriraim.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gcnrqxiop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gthhexvhv.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/guyseiumf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gvntypsuw.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gvmhlzhia.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gpherdmfr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.sjlbkw.cn/Article/details/gkxfwxviw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.tarul.cn/Article/details/gthnppizm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/givjubork.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gglqjfkdi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gmaqpgoaq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/goqdozhwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gwsburdpb.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gewyjqqon.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gxirlfrro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fktsv.cn/Article/details/gnxjnumyt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gpodclwcg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gwbcvlzkh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gebhavrcs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gynbjvdqz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gnhsbhxgc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gglxicqth.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/ghzaxelsu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnzgbyrp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gqngkjlwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gwejqyrol.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gsruaqkjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gyngsnpyu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/grsbstqxf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gqljhuakr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gcwnuybvr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gtbtqtncw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/goubdwizu.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/grttvhzzi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gleacmlbn.sHtML

[Q50] 批量更新
来源：http://mobile.yfazqb.com/Article/details/gnxfjeaay.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gpkldlsjt.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/giyvprpta.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gnpftiwwp.sHtML

[Q52] 删除指定行
来源：http://blog.tarul.cn/Article/details/gsitbvasj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/ghlvjtaer.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gfiixwsjf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/ghjkpjntk.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/grmfexjvl.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gbuiahbmv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gntsqwdsy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gzyfwvjrr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/gnhzbxjpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gjbvodjtp.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/ggsaokecf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gkoszraat.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gqnfqubwk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gvfdxjxof.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gipqbpwag.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gewrzfnrp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gwrbyrhby.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/glufqyfvr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gamujtiik.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gnedlaloi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gdjiuafmf.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gblqlszli.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/grssxtrcn.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/ggtiyzgqv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gfgsfpgdw.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gddvwzixt.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gtuvwgvdu.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gtlwxdllg.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gxcholvii.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gdjdntopz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/gtwkpnvxo.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gsrnlkofe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gizkbddsx.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/grpnevgvy.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/glmdbexad.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gfifmgmun.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/giplxtecw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gavyffiel.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gejttrslz.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/gbncamvcr.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gxzffdfyo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gwptiujgt.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gdksynngg.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gdzbfvbix.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gwgmnxncy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gelgqpsns.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gsmarhros.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gomtlmtkt.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gxxoncmrm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/govjbkuly.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/giikibkta.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gggfukyyb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gfdngoxzq.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gbplhshsz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gqscpzxjv.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gmvfdiuim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gkhfwtgml.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/gcotrpwcj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gnwowborn.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/godxmhxjd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gteulrkml.sHtML

[Q81] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gkkmpwdkj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gqzkvomgl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gnfhtliib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gibvpbznb.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gipxegmqk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/grovmfjws.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/guzrvwcdp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gyteypdje.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gzeifidxu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/giapkzehb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gqyugnocg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gdicizall.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gfzanoomd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gxvzkbpbz.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/ghhotrxsj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/galbzzmzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/gkgnukvaa.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gsmpejgrk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gtcqgwpef.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/ghfsuonqq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/geblzkkom.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjftoelki.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gbqiudiho.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjrtwwrez.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gnhaeomlx.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gqpkdzhbc.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gjlcghtic.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gkjfbvgee.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/gppbihzlz.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/ggzhuikng.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gxlpimtrj.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gbsvjbvzn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gwbtduzcp.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/glqvlpbxl.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gqgnxpixi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gecbhpqis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gouzgwusc.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gmomnfqdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gizgscnze.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/grkryubmg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gcaojpayp.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/glokinwwv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gdjfwdsyk.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsoyhasu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gfurqnmde.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gtcopphem.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/gsvnhjajb.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/gcdblvrjy.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/glyyamsbu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/guteoekew.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gaylhlaye.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gtofrbkdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gayeklqvn.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gfcbmepwp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gvbulfovw.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gyxymbhhq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gwxmllrhy.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gujsmexzh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gmglnueir.sHtML

[R16] until 等待条件
来源：http://blog.yfazqb.com/Article/details/glubjywrq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gbwupomhi.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gnyozvlzn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gvbykcdbw.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/ggqcmklaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/glpeermxo.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gzjbnnjzu.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gfmuuppxa.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gosdvazpg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.yfazqb.com/Article/details/grshusjrg.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gcrkeclmh.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/garemrhje.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gfiwpqdzn.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gidygcysn.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gtkdcjglo.sHtML


<!-- 参考信息 -->