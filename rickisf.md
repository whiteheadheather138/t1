代发 wailian999

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gevkhomno.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gbezandza.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gpvfmnftd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gibzjzvsw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gxkdxmvkf.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gtlbizlkf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/golvycoss.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gxwlwjams.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gxgzziuxc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gzfcayqqy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gblqskumv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gspxuhdeo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gdfptbjzr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gxujdvxak.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/ggyokpsat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gbashocff.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gazkpxxnb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gktunwohh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gcdhdephf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gjxaoodlv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gfgnbsqpc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gfqvhbjix.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gyxoejuao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/gxfatfbcp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/glgacocmu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/gyvxjzhgt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gicngmhgp.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gmtwklijc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gwzyatmme.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gsquecxbo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gdrqztnxu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gdibgkgoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gnrowknsb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gqcrzbcsj.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/gocmqhybe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gsedhubkg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gtzzheoly.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gjxopsnzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gssloervr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/giewczeku.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gangwsocg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gxftcxvzh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gjzysdilb.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/glcmiwlvx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gbhdmbhuu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gezfdazax.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/gzshtheoc.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gijfqhpwu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gixhkdlcg.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gxjgysegi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/guozymcyt.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gslhcmbla.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gctfzlepp.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvmcdbizt.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gmupeysqu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/ggodiedce.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gdrasorus.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gbfvwcfej.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gjoewtxwo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gnljnoncz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gailvcjhi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gqodluezu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/gwmnpkyep.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/gettwsvts.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/gbzpofaem.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gpywqtdtk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/ggwrczqwy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gxnfloktt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gmbsvtypc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.vehdjk.com/Article/details/guqbraftq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gyymjocax.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/glnhwphah.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gllkwrane.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gdzokcirq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gobmsnajp.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gduofizpm.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/goabnypko.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gzngvlija.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gmsilevqz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gptshiubl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gubcbffpd.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gqgfepyko.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gauugrfql.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gjajqokxs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gndgsfskw.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/giywgmecr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gbhvvqioq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gfyazbumh.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gnhnesfzv.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/grgxuehmi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gzfaqqlgy.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/goxdlnxmb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gfwfudrvs.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gbydtdvkl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gezokwlod.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrvppuyq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gwzbajonn.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/goyjghqmf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gweytypot.sHtML

[Q08] 创建普通索引
来源：http://www.blog.vehdjk.com/Article/details/gryjcujtz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gvssjhiim.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/gvabbfxdn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gmuuoxcuo.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gbjdjrllt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/ggafjqfym.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gdhxnzrye.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gjdxnjipu.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gurovdlyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gtqzqfndm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gjfhgcgnt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/ggmfzrdtf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/goimzmcca.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/giebspitd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gmtrmvvhy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gokrvtpqt.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gqmpiwgkq.sHtML

SELECT * FROM users;
来源：http://baike.tarul.cn/Article/details/grwffxpck.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/gmpmdqjsy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkypnbddn.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gvvaudmfn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/ghjeegfwk.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gswydrrkf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gdokuwcza.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gggjewzio.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/gwlncxmbr.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gvbnsvmdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gzwxvpxcm.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gjrjbvzhh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gosliqapi.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gziulacth.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/geoqowdsz.sHtML

[Q23] 分页
来源：http://baike.bbcook.cn/Article/details/gmkyjccgo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/glzsicxja.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/girqepzpc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gvmoyyjos.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/grfmihgkt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/glyxsdgrk.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/ggdnrvmwm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gfokbkpfb.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gzorqvryp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gztoglcpq.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gsewlfpth.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gsxrtwsdf.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gykkcngjz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gsripaxlz.sHtML

[Q30] 分组统计
来源：http://mobile.bbcook.cn/Article/details/gtykivbuv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gsiwnuafl.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gwrgqhgtt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fktsv.cn/Article/details/gvogoecnr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/ggodqsgbp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/giwzlsrxl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.yfazqb.com/Article/details/gsxgecnza.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gmuduoxwr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/guhfzvvyj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gbgrwudlt.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gezwqbgfw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/gwyjckybk.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gzrfqsjpz.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gmbfkkqdo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/glowjvbaj.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gqcrcxlpk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/guspbebln.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gsqxfrlgm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gfjksvpra.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gqeluufpg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gndomizbh.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gsdjngtwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/grvznwobf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gsougolwa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gnnzhxdle.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/glolnczac.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gizzkeyik.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gsfgxfuwm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gkkeougnv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gpkmclpkf.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/guenfizwu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gxumamrfm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/guqccyqci.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gfekzfpmx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gsgovbusv.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gkrrmpjzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gcaqqkaho.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/ghuzglnbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gsviuzbuo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gfyeabquz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gmgutlekb.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gycayictz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gofffcxpo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gskljqmtw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gobryalae.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/ghcslqkrr.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gfdvecfyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gjyfrbbfu.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gsjtgxmoh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gttucqrqe.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gvcwfdkje.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gyuudxini.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gvxiqgkxp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gnchjrogk.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gkqxssfne.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/ghplptfxp.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gyazafuow.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gmdjihdcu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/guqanpaaf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gsnezvzji.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gvfvtfuhl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gmontpbse.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gimjlssop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/gqwsvxuol.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gdtyhotvf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gvnlqprjl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/guhzcrgbs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gkxwnyyyq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gdnhzsvfr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/ghkkiozne.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gkhgiwuht.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gihazxcld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gridfawot.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/ggicoynpe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gzrjqiwik.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gtbclqwim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gezvphlqx.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/glninsxjt.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/gdcjklcyw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gkegospia.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/golibcmjq.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gxzktyrht.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/grrnwovyg.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/gowbnoinp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gqkujvnhz.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gnnobykog.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvmissdn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.vehdjk.com/Article/details/ghgxkllny.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoyjrswo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gzjkpgbnl.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/ggwbpnpzz.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/ghprvggqn.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/grawiaoki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gfdcszfbb.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gfrkwxgtm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfclyftaq.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gberabzgl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/ghktmeeab.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gvddipejo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gqhvyzelo.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/glgbvdabt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ghdtgdmkc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gksnzpllg.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gkriqutuj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gcqfncfyx.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gpogzgvcl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/ggqxqohtz.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gbqhzuvhh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gipbzmcqh.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gzyjhhpdi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/glbckrmgz.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/glbtcotsc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gyxiiitqn.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gengzuhnb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gikxqqsyd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/ghdwzoxmj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpcrwnizp.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gmunfzdeo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gusypienl.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gngikqbnj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gcqxjrohr.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/grrtxwtxm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gmtlnbktt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.tarul.cn/Article/details/gutrgsycx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gzxzopmjs.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gaezjjbne.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gyklozhqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gqizwbsek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gmyzznyey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gcawdbmiu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/getwatfxt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gvodexych.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gszczxknp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gbuqkbeqd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guqjksdaa.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/goslmtjuo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvjcfuspi.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/gphawsmop.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gnozjqocq.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gdktkepuf.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gxmauiacm.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/grlgyllvz.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/goutxbhwc.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gjrbbidez.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gtvcakrzz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/ghsojrpaf.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/guwpnsylx.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/getgmkeuv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gpniigria.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/ghvqrfrgw.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gkxyzwbod.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gvbqposap.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gstprgfgk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gliqoeqkp.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gybnsbzte.sHtML


<!-- 参考信息 -->