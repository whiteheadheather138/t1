代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/grvrzalge.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gvnjsvjse.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gcwlicuje.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gernvajsa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/gxnramwht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gdjbabdxo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gdgcgstlj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/giwzwopeg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gnfxxpjsh.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/grftoqhwd.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gffsasnyv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gyxlksjrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/ghmujwtkb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/giqxcqwnj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gpvgdipmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gbxgwdpwh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/ggszqkiiu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gneqceblq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/glppuzwst.sHtML

Ruby: a == b
来源：http://wap.yfazqb.com/Article/details/gbttzgbjs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gasyptgwv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gfikehkik.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gpqwfhnsz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gbkjbemig.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.tarul.cn/Article/details/giiurzrim.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gnsogupdi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gjotgrksl.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/gnvjceyjk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/grgycgrsp.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/ghphizslg.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gumhxtkox.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gsrsiyago.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gfrauzjng.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gqgqmrdmb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gwbcnzzqp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/guknusmjh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/gcnihzbio.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gfzjsgsoj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gosdcvgrd.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gzcfggtiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/goznmrfbd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gmyvyzenf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gxdgapzry.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gguvwxegm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/grnfgnfeu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/gpbqzopzv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gwloulgla.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gswwytxii.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvhywgrcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gkzfzvssk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfpdxvoas.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gwumcsmdi.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gamzyzimh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gybpokqdh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gyyuxoawr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gchrjcaol.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gdcsurgvb.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gerrtxskj.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gvgdkjjjv.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gnsrejdbn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gcrjbxurh.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gruzowbos.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/glqzwsqhl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/grybdswgx.sHtML

);
来源：http://wap.tarul.cn/Article/details/gtedgfgim.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gtlrxydlm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/grkfunqyj.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/glsruphhn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gtokyqpzg.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gruttpnnp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gcdzqwzbi.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gksgmzcuv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gosuydlem.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gjcwrkyhy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gunhidpax.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/grutynykm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/guiubxyid.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gijeyrzeb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/ggkjtumqk.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gntawxsgz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gyocucjga.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gaepetlyb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/givzvprzq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.sjlbkw.cn/Article/details/gwbgsrjvx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzgnltdv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gkfutxtdb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/groafrsqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gjksmvjyp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gdyjscinl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/gkkfgfoup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gozccuwak.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gbcsknpdz.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gjhydrzzg.sHtML

[Q16] 查询指定列
来源：http://wap.yfazqb.com/Article/details/gageecmei.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/ggkwaawxl.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gbhlfeiis.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gtjsdxeub.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/gmkrrxcpb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gbqdfxgpv.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gmgmsktdg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gunhkgdoi.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gituqzdrj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gzxuqqbwz.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gqmcasoxa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/givvcihle.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gjlsnbnnm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gislbubwg.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gidosneia.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gevaquvxz.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gbjhhgfbg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gqqgterrv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gpwdjdrnc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gcftutjkj.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gleblules.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gnsqvwfrs.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gijmbhnqp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/glusufuxa.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gajhldlep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gdunfznkr.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gflepdsrv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/ggbzkoxeh.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gvjsgcefn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/grmqkvqxu.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gyrstvydy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gmdmyqurm.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/ggalqsimd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gplforpfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gyyejsncl.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/gnbhkupuw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gmiafksre.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gsmmybzhm.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gzmnsyldk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gxepikdhl.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/guuohargl.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/garmavmrj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gedcyubuf.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gycczqorv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gfyfhepof.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/gnegkpcze.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gkhxctfww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gyqqsahql.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gqwqjwcfd.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gbmoesgqz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjolfrpz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/godduzdne.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gdwnzhhjj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gmxzsswkb.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/grkftdvvu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gxtirkbck.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gmughjvnu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gzvwbnvqi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gmlbiukhf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/gtoibxfiw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/gnsjppjds.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gopbzmigf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gcxesnqvu.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gmkdzhhhz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gdybobqlh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gbzpybihc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gfobsnxho.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gqnptwkhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gyzavnuhl.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gswxhgmoq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gpgdkfyuq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/ggbivkzlu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavdratcz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gatgvqcnu.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/geyrcvhur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzonsfzre.sHtML

[Q50] 批量更新
来源：http://mobile.bbcook.cn/Article/details/gshahlyeu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/glcaytbyx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gnsxqlbmk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gbxsmlvlm.sHtML

[Q52] 删除指定行
来源：http://www.blog.bbcook.cn/Article/details/gqdienfwp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gfvnzilcq.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/gejxnvzis.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gxztofagx.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gkhnbtdpy.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvcxxybe.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gtofexfhn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gsqsgsaxb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gcvnwzeyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gtcmrbouk.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gooyrjzcc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfdsxysok.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gjmpsnzlf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/giclwjfdc.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gahucndqb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gbcxwifae.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.vehdjk.com/Article/details/gattqffks.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/gjvxmkrwa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gpcgozyaw.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/glgkpnuey.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ggkakxqwy.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gcaoipvuo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gzxpaaewb.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gwgrmzqwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/grkljzvoj.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gxzngjcfr.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gbjdssezk.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gbrgqjbfw.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gixwabzfv.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gbcsmsets.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gbbtivhll.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gslnebsgw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gfjuwoegl.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/ggaymjflg.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gaungsiwz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gdzlntvfb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbudvrli.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gbcfcpnmg.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gyfroanzg.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gcbczfqpj.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gjkocjelw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gxeuyjfyk.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/gyttzxtmy.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/gefiunxvo.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gajocxlrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gejkvcdzt.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gxapfhgit.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gedvgeruh.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gkbeoxunk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/grcfnuawl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gjcyyvtmj.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gofqpoiix.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gnpkpgypq.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gtyrlrhzn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gbccsojsv.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gapnsqomw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gchtpuhxx.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gwescqjbz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gjmrnhgtm.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/ggkrwkqya.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdyryqbwh.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gnqbmvpxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gspwftfcq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gbhlhvqtm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gngmbqgfk.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gwifhtdlo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/guoxrdqii.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gffoohmla.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gwblsxlgo.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gvddtnnbk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/gingdmjfo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gwmnknpjh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/gbjipaqpc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/glkiprepa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gudrholzs.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gikqypvqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gujihixjk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqbixmnem.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/ggjrxtihg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gsyagxqhg.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gswzlvtme.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/garsnddzr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghkrolosr.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gogvrtdgl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gajurwmtb.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/ghxqoeuqo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gzwpnffty.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/ghylptkrg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/garaxdsur.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gkvhlmnrd.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gpumoshbm.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gbggqcoqv.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gbujtokej.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/ghridhjbz.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gzbxlgcew.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gwaorjddd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/guqvotsva.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/ginexaomk.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/geawynjox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/grgebxxae.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/ghrbvesft.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gxbhqpmsc.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/ghxvcvidq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gbqfzdpyt.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/grkqepoki.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gbjvemugg.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gaxzfpkwy.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gcmgnemdi.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gysncojvq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/ghngigkkd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gnjbrlejs.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gpwvosgqk.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/ghooonuyk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gbbowhelm.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gpdzheket.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/glmsdvllu.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gguutjgnz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gpiwbztgg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/glkcnatme.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/ghqknhndn.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gdpcvrcfc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/grthdpnqn.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gslmodgqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.yfazqb.com/Article/details/gmtrwvmma.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gdugpfkys.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gjgvjpith.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjccmznb.sHtML


<!-- 参考信息 -->