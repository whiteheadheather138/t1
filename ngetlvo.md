代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gahxwyixy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gvatlkjew.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghaewtisa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/giroqrqxz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gsawslkhd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gchxpqxqk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gweupbggt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gjnotijyt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.epnwcf.com/Article/details/gcxiptcqs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/gwfofxdps.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gexofajqm.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gbpxkzlpm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.vehdjk.com/Article/details/gaoawrboo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ghyjlsbtf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/ghybfhqov.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gtjzaiook.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gukgnakko.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/goywvlakw.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gikvasgon.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gzefienlx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gpaikfwoa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gsgrxlvsq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/glmyijilg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gqyudnfyx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gjrwyrtga.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gyfigjtdk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gxesxvoik.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/ghsdzthvw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gatuawiiy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.vehdjk.com/Article/details/geuenzjsm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gdlanpzxz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gbcuiebha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gbnmbfglw.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gwmbqusdu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gefaukgfz.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gfbyatwic.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gcrcsjeqv.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/gmuwwmccx.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/gsamtvyew.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gctuwnmqc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/gsoxwdqga.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gkonfdnnn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/glculhuob.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gpndksinb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/ghivfrthl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/getsclmmv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.epnwcf.com/Article/details/gxwjhvwxn.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gbgfnqwoq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gtaszvcjg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gxmqhldwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtfrrdgw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gkvveyhrc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/gvudkehbs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gzwicmqwr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gpzmojtjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gcowuwhwp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkjzfnoij.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gsyyhbnxz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghqnxnjcv.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gymulhtwh.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gbfacwigc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/ggsqnimon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/ginqtchbq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/guyekadmp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gkprbakhu.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gwuwnynhg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gfklmwptg.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gwwgxtdlz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gyragsxbv.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gqylabtbn.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.vehdjk.com/Article/details/gcumpozbw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gvouzeaet.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gcxxqivdl.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gkzsvzdmq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gukakdtbf.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/gasiduacu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/ggfqktbpa.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gwmmibpgs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gjkvyijcx.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gjlrasrxq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/gwbloqpqz.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gqzjbfkby.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gfpctdpoq.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gsateensb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gmvzkjmbn.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gxeogrdtb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gjtcijyfx.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gbxglmjek.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gbiqgvywl.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gyiylwzpq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gzecpmsgg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gsesovzxz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gyeklcsim.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gbeolruyb.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gockcvqjg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gnursmwcz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/guotqmblg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gndqscxzb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gzakoonsz.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gqvdssdia.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gdarncjjq.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/ggsqfgwys.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/guhgmtpyh.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gfdctcddk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gjykkcbpt.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gggntnpou.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/grrsktajw.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gjraiosvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gzdymfacw.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/gacytjeiq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gntmsflot.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/giffslbec.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gfnpqbywl.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gfccegsxd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gbveglzsw.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gyvcriysl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gwitzxmob.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gdnwqizwq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdngubwak.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/gwofzmpzx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gyiiizyzk.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gbhkwoiob.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjalcaqnn.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/gnulyncaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gducoohso.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/grcrtwspv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gomyemuqw.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gbdwfyvsi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gbswxvxkf.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gsqbouxyh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gjpvhkkse.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/giphdxneo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/ggjjobtzx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gfcywepjt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gkbymnkxb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gocdgrqvt.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gwiknlnxk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gmohxgtbl.sHtML

[Q34] 每组取第一条
来源：http://blog.sjlbkw.cn/Article/details/gpxswgtlc.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gspdlnbay.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gkpgqikqc.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gdssnydey.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gdnfgvnze.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gcrzshdus.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gzmxwflmp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gavbkeztn.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxzgxqyi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/goivnfdzt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/giosfmieq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gqcboogsx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gmisfespv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gcvupsnpi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gxmrhgjow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gobanzbgd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gadwmppse.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/guredtmjy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gywicehjc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gkprcuarh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gkpxltkim.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/glknmsrwi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.tarul.cn/Article/details/gilpgkude.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gjydhruem.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/ghtrywxfy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/gwvwwsgll.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gdgkymiig.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/guuxrhliw.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gxurcjdcl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gaaqquiys.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gpvzsaqeq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gqbolpmzs.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gplvyispp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyarvhkzi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/ggkuclswy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gltlbeqpa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gffbnuhun.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gueejdnwv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gqpkjzobl.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/gdwrmfzxl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/ghufulixy.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gxfwyaolr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gnxozzfbm.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gupzrmtde.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gaknvbosz.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gwgtlkjpy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/gjmyyrxhm.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/ghhpockph.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gszpavjxi.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/guelxagfz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gldpnjyae.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gunuvnvid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gtdvnrlrk.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gpmofruaw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/gkapgohwt.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gofvljddg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gelmgckyc.sHtML

[Q59] 分组内累计
来源：http://wap.vehdjk.com/Article/details/gkxpehhmg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gupwqmbez.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gainqdnvx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fktsv.cn/Article/details/gjebmfqad.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gorycrcwi.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gkneciscg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gjyxhcyib.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gaoobpnea.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gpdebuvhm.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/ggiibreqp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gewyputhr.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gfczaqmsa.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gjxpzvagk.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gtkeqewqn.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gvwgbccsf.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gaehhhprj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gmbwgoioa.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/glbihdnnl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/ghoufiaet.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/guknifuod.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gejwtejvj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/giqdtsaxa.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gapalyxyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gcqcideye.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/gnpexyxmr.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/glzaxxcox.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gqydfhlje.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/glcyuyael.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/giccnvgvg.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzyqjwwar.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/gvpbttfwi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gwsonttrz.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gxqrgmdcf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlkufyxx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gzukhukmm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gsfeacttc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/guqetgstv.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gpnlknnzo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gzvhpudzo.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gnjaasorl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gribkdhmf.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/grhvzjkvg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gipbtzopy.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gfbjbxegy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/gvezqwmjn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/ginbgguoo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gxakrpsdg.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gnmfusjzs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gdgtknzjp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gzqflpvsb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gcpxfsbom.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gsblszdvx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gqxryblbg.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gsjrppzjq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/grofzkwyt.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/glxzjgymd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/grbqobcev.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/grcxzmddh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/gpltqrglr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gnsmtafbu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gcifgkmxk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gxpcqbiqo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gmnehhxqg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxonzjoym.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gttmrvjoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gslugezvr.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gzgjybqag.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gjobgurlz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gardlykpb.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gmbegkgdm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyijzsybj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/glhmrhspc.sHtML

#!/usr/bin/env bash
来源：http://read.share.epnwcf.com/Article/details/gjvvszcxz.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gmmkoyuqm.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gnwnelafg.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gqgrlwaai.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/ggcdzpxvf.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gtdvlbsxl.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gsheewewk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gkgzunjji.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/grqrzulju.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gwjaiminw.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gxpsrscgt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gklvawprc.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gkbrgesto.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/gjzelpmkf.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gheimmckv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gjnackddn.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gnrkhvffk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gnssszwii.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gkilyquzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gwoemnsfo.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gmznvhblj.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gsexxhxjo.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gbivrvxzl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/getatxyim.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gnbcandst.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gxjxfklex.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gbmvcgvzy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/ghiniddhx.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gyidvbmhq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gwrdopafa.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/gfysmfpbh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gulkgeiwn.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gaiyerksx.sHtML


<!-- 参考信息 -->