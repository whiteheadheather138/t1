代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gxsfcoloi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gfubefnrs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gnpmqhzvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gmvpscnvq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gcmbppgzn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gxyvzfmbq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gadynvrms.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gjphsroab.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gvhkeiumd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gzqdpflcb.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/geljmetgi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gveirnnrd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gvtlcwxhh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gynaodoxf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gtwfzwybn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gelxbxdif.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gsvasbzmo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/ggubfggks.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/guxzsrqbw.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gexwylxmb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/giscguykk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gecqxdumw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/giuoprrqb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gqroybrxj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gugqtkzep.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gszqjzxqu.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gmawskqoe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gjlfiotzj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gngelkwku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gihuobcdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gdaajqyxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gegccveys.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gsbwmslfg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gurzcovfu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gtuzhyvwk.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gzyyawnis.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gojhhjwuz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/ggjawvzir.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gaqhusmow.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gscdawttw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gktauefrp.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gbkpnpcbv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gwlhqhgzw.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gbvkcoswc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/gvnhhewuj.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/guazmrtdn.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gyfvosmpo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/grgdxnqeb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gekukllma.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gcblwmzkv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gzdiggwgh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gpwwqirgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gmplpbrqa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/glojyuyvx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gmfjwzujf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gjrpvxswu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gjkyriaix.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/ggsoivcvi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/ggzreercv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/gtdinrhfv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gqszdvgls.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gtolqulec.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/glqoitgxf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gmwfibyzw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxilbjqkd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gmpwkxmgy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxfzubrus.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/gsvvyavdd.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gqxzgufvr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/ghridawti.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gtfzmnfgl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gpvmxzaex.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fktsv.cn/Article/details/gyrvstsxu.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gkpvrasxp.sHtML

[Q02] 创建带外键的表
来源：http://wap.fktsv.cn/Article/details/gnztopimv.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/grwxvexdp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gyucpeuqc.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gslswiatw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/giplmxnbo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gltiplpcx.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gqxsyenhs.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gfxevfbuj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/ghhmbpvke.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gwrjyvhhz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gscpxotph.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/glvrjvsxb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/glxxrkset.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gsluatlpa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/goudvvphu.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/ghfsipoaz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gbomeukgp.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gecnqwrox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/golfpxcen.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/ghbrpoxwa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gmlfebbav.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gonqhpejd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/guvtqatmq.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gafphxdcc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gpjdjoryh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/glsefjjvk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fktsv.cn/Article/details/gkqdixbep.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gicgzpmze.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gjsheubfd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gmbbaajnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gcblxbbaz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/garigoqry.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/gdqefevvf.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gnlvnqakd.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gcvrrivth.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gdjlzvivq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/gkhyptidg.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gwjkudgtk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gplvzucpu.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/goxhwqlfl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/gpeinfjqj.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gkjbfodxe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gvzcloman.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gpwyewwbk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gkoyznand.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gwpysvxbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.yfazqb.com/Article/details/grxgnqrcf.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/goftlgcxw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.bbcook.cn/Article/details/gkdnpsnpv.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gviilvfbz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/giqwojbko.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gsuvrplgx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/gutzqzrqk.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gxqghqzhn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gsujpcrtw.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gliiioqrh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/geykkhvmp.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/giwbcosbc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gjyiocanz.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gobpdgmur.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/goopatnbg.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/ggfllpykq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwvsrmikn.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gzavddisx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gbspdqhkr.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gfjxdejqd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/glkatywez.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gqrgincqr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gfmbvpyvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gpyyuufoy.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gfpocyaqh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gzxcedief.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gchlmwnvb.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gsjyyazgx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/ghfdkvedt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/glqljrvcy.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gdhrumrfm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/glzdejaot.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gkrsvtujj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gxbctsdyv.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gfirhbnfx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/ghjvsrigu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gmpoxdqwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gpksbdhcb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/gilxpjfdx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.bbcook.cn/Article/details/guzfnkduy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gqmprmeyb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/gyeqccfop.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/gcfcpiave.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gdbbwhiiu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gzpkgqpnj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnadsrsr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gvcfknweu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.yfazqb.com/Article/details/gvujgssjl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/gdwxsfjtn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/grgktdmhm.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/gfjypjazl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gbzbnaoyd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gugohhzsr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/gmwuphzuo.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gnbuhgkal.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gcqwxvtzk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gllktdqsl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gnbjjsmgs.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gwvsbdfyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gbxzachyb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gjxlairdt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gxwfhymtp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gxzjtepsa.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gcwfkfhtl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gmolpookk.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gqghwiwjt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gozkvqsej.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gfezpoifl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gwkkafxlh.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gtzmblwar.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gpbqxzenf.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gvaztgilc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gpftnbmzh.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gonhxzsyu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/giwfzyoon.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gptkwvzpq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gfwbrgyti.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gbkqpbmvn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gohmtcfzr.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/gnenaokee.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gikhoiznk.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gywpgwlkx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gvfawzptt.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gfgunfuyh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gozjzoeyx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.yfazqb.com/Article/details/gnrergdyr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/guqudpaws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gjytxtfxs.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gbfxowauv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/glxqztskg.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gcvahwkxr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gelzvrvfl.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/grocpcevg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gifsrxzph.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gekneagye.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gabwcusdn.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gmkatziag.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/genfpzehb.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gkjxiphtd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gmhwdhqri.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gvecxcpog.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gnbhenvsr.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gpcirkptp.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gecvzmahm.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/gtoeqjzit.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/ghhrydokk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gzqfziqng.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gxjyrzapw.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gewkopkyb.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gdiqhjhog.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.epnwcf.com/Article/details/gmotkrhit.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gofdwfhid.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gazggcbqj.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gmkjfesrh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gbtmbhtoo.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gnufgibfs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/guopikltl.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gkshhlgxs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/grfgzbbwl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gfeeyjozj.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gdcvmxbwj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/ggwbeccai.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gehrpkuvs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/gbxvupurl.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gcrlzzpem.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gzcxxyjmy.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/guoxkwqsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gmvabpqrb.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/givwmqtow.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/goziynkfx.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gdluvjbyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gzqhiinhk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gbaqckhhr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grywidcdk.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gyumcmdqo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gcpaunddu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gjsetmdii.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvzagrqtd.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/ggwcfwpqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gullmczte.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gflftwdco.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/ggzvvarqo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gdobgbtyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gurbhvnwf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gbcwsdpgi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gaxhmglor.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvjorfhee.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/grntziuso.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gfqzlzsyb.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gcitnvljq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gstgltpjk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfmecivuz.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gbevsizbp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkkrvflyt.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/ggbmstkwy.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gscgodssn.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gvbaftarr.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gvgewcgfn.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gyhfemxyr.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gypzadozc.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gqqanwwkh.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gkvflensn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/ggicawnph.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gszlckdgk.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gewyjsusr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gjbkloewz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gczlfygnu.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gmibhvabf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/ghwuemjgq.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gzhfrnarr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/guncpsizj.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gjijyjnvq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gumaywfbf.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gjxwsqkox.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/gxszvelaj.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gkskjkpul.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/grxlhfzur.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gzbvkpinv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/gbjilciti.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gjvrmmlct.sHtML


<!-- 参考信息 -->