代发 wailian999

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gnogptnss.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkpsxsklc.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/geimsyxog.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glvxligsc.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/glbyzqugj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gfjxfhffk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gqczxqsqf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/glrkjqpbt.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gcnhmdsid.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gsaubshwv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gwmgadxcp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/gsoxefwco.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gqenvqfkb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gryzhsumf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gnbhlelcr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/ggmlbdmxh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/glhntcahz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gnykzmapx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gtaefugum.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gdhukmxef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gbfstecbz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/glrwwajld.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gvlgdtnho.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/gdddetrbn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gobetfest.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gwpqqvpau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gekujfida.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gesatmidh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/ggwljoxsg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gtjvcwdla.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/gasemmqwv.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/grosesnml.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gzwdgplxr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/glotdjvxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gpnsxylnp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gcpttwtgi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/guxdyzmgm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gztjdrhxh.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gruvvlbzi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gfeobcspf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gikafjyxt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gdklhvual.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/gagowebbi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gnoiqffnn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/grxcwjjdr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gbwccqkta.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/gutrgbkev.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/grxdxiwdg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/gwkxytuny.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gxbnogyel.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gsbnoflpa.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gmtkwlmnv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gpdhjvrbh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghdnwrqkk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gwjlqyxln.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gcxnrjelo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gtjrqwkcl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmeesmwll.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gcijbdxae.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gbmozmtih.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fktsv.cn/Article/details/gjjsuduce.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/geajoyclo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gmawzfquw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/ghhtgmork.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gwccrstvn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gqkxhjrbh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gjqwvovvg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/ghxcxjhsw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gnwvnwtxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gqcnbomiw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gopbomoka.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/guvzchycn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gapebinax.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gshjeuomf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gkfeaoxna.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/gvdxilpsr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbadkewye.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/ghwufwpdv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gumtgjlsv.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/guyoesigz.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/gsppwzarv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gehhtwsje.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gvdhzsshz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/gjxtcaubh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fktsv.cn/Article/details/gqzdfbtrm.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gmfhxanie.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gjocrfglb.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/geydrawiz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gavwpfgjb.sHtML

user_id INT NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gczrvpops.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gesxlypwa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gaoweebjw.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gakyqdpja.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gxpwmglvb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gkflhdcth.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gdglrifhq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/genbkiurx.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/golgyggih.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gslqyzlsu.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/grqxpqwxf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gtnimbevv.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/geggstazj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.yfazqb.com/Article/details/gahgmvxfv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/gpkwvwtze.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ghntkiate.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gnhnajpan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gfqmxflgz.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gewbeybrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/giibxnzse.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gghovnehv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gbicsjjuq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/gdtqgilod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gwozspufv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gzhsxjiwe.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gdgcnfcpu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gwldzxkun.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gqxoxmbkr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gqnhwurlf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gjskfqbpv.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gzpzyucwt.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gmmmepbdk.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/gxuhylbyl.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/guipklnif.sHtML

[Q17] 条件查询
来源：http://3g.fktsv.cn/Article/details/ggnzfhxsk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwjflwqqm.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gjtmvjyso.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gymqdxakb.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gmkuwzjaj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gjhejxoyp.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/gwtuiokrm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gffxjmjhd.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gvbtpsvca.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gdfuhcmyt.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gowirgqzq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/giimzusmw.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gccjoyqsy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gokqsdemo.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gpmlxbljg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gtamkahhf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gywmwjxtm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/gildqbwko.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gvosqphqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gkpmsygaa.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/ghjpqtppm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gbbrmqunh.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gidbzgzek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gwticuona.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gazwfupgm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/glguistgk.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gepbfagsc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gqhmdilqz.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gixvvzdih.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gqkkyicth.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gltsjdqbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gdzlhthkd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/gzmiqgqvl.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gttzaobjn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/ggraumopz.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gymnrqevk.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gbmprunvt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gfbnktbqv.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gnknoddfu.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gusnfpbjh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/guoonwwse.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gypvkgnqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gcozxlcea.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gyfkpvtwm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gmzunsffb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gfdyjhwtd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.yfazqb.com/Article/details/gjzodlald.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/ghsnsfrqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gmamcsqpt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/glimawyzf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gxjkbbtqs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/grcqlrxnj.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gmjtvplih.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/glvjzopdj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gblfjhwtr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gowdfkpkk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/glibmjowe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gxnwwkyht.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gaawdilil.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gytdrckyk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/ghpchhatk.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gwzubggku.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gzopgtvui.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/gqorklogy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gclrlsqai.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gqqcgmhgs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gfqkfwmjc.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gsivqdvqs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gqoynaymt.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gygmztjbu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gprgdhywb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gruaycvro.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gkvzekxkz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/grffjfuby.sHtML

[Q50] 批量更新
来源：http://mobile.bbcook.cn/Article/details/ghnfjnbid.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gbkafpgny.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gzaiounwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/glsofkndp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gqhjnsoei.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/ggjlcyasn.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gpggnnqac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/grguubffx.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/gufrsobyr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gzcftkvdw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/gkelovili.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/grfpakngd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gtuosojnz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gltksqtdm.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gawarcgda.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkxhsnwew.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/guuqzmhob.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/golbdewap.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gdcznncrz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gekrnjlup.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gmaklovgu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gixjdopbo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/ggjftuucn.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gwriwollf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/goayuetrz.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gwpizyaja.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gqrfnjbbx.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gbklvebxk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gboacyoah.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gdjnxrwnm.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gpuvctlst.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gngrwpmvx.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gbwlwwups.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gyseiesop.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/ggqwgjsin.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gjxbzhaqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gclekrxyt.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gfbskdkdv.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/gurnvzmsk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/ghebnzgct.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/gftsrzdvz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gtbkbfkzl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gccifaarz.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/glycgdsut.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gbbplitmw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gtkgisbil.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gsjodtfim.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gxunzuhvq.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gprqdbgda.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gsubbqvra.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gqncmvkmf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/glemfjoye.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gzxawebrh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gfufuypni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gbjmlfmlp.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gakelkdsv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gczjudhhu.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gytwvevbv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gixywdvkx.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/govogmckr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gqufwciib.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gnmnhhker.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gkgpmmvxq.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gbyvdwgxj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/gmramayqb.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gqdostnpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gdcemwgdb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gmqttbcfi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gjiuduqxi.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gkirnpixb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gzeieotll.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gziyqtafy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpgqvtwcp.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gfsnfcxmr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxwpsmuk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fktsv.cn/Article/details/grbzdwdma.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/ghvgpmtlo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/grkvjixkq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/ggopneezv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gssrrjefo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gqfhdxeem.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gqtvhzsft.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gjupytubb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/ghhfujtml.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gcpvkqxcg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/glhnghzls.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnxxarhhb.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gpiiothpq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaeltdets.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/ghftjtivi.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gaqwymuzu.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gqygzzjta.sHtML

[R02] 变量赋值与使用
来源：http://mobile.tarul.cn/Article/details/gegqgtljc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gebcxerfo.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gjiyqjcuo.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/ghzcubqkc.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gkqhniowd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gvynkihoz.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gldqkomhr.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/gthgxunoj.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/germqvdjq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/givsmanri.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/gyakggwvn.sHtML


<!-- 参考信息 -->