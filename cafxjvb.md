代发 wailian999

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gzazatdsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gqdxbpyfr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/guopzftxh.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gzhljxmsa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gnviiuvdw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gusqixisq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fktsv.cn/Article/details/guixcckul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/goxmyhush.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gmbebjwep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/ggdnvyyiq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/glstdokeo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gcyecqnse.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gbbzizmai.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/glnsbhiuq.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gtiacvasz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/ghrptzynq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/gdkbyoixg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gmmlcdtys.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gtznkefmk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gidnhfsoz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gvrqfwdke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gweoqsxeq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gjyaeetah.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gryvuugwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gczbssmnv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gcxzvlxib.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/grehboprh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gbdhikjqn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gzppvptjq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gurkliral.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gucuyojjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gjfmlcjes.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/gromrhosr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gsvubqbnz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gkdsynugj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gvpelctlo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gdpdxrekx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gtfncvlcg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gkoxzbajl.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gqlmaboay.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gxqponxar.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gmwghvruc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gmufpkkbj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggzrpnjpm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/gopvwvrak.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gtxsxbait.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gdxlevaff.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/grwiitxnw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/grlofxqgd.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gcvckenwn.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gvsvqldub.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/gdwovkyst.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gleslabbt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gbrpktgrl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gyqxfutco.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/gqgaghevw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gsvinsoih.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/ghvbdmzkz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/ghapyhaqt.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gxfnqxzii.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gjiqrmeph.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gokcqjycs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/ggsjxrgml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/gninzjmal.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gftdrexvd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.epnwcf.com/Article/details/gnvkdzgii.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gfblkwhoz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/gcwdxmxhe.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghkmdksie.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.yfazqb.com/Article/details/gtbjrxdxw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gybxkxzws.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gnezekihu.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gsnsvpzqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/guatrutps.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gbtufbfyw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/ggzkblhui.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gmxmkdgcj.sHtML

);
来源：http://blog.tarul.cn/Article/details/grpubuawp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fktsv.cn/Article/details/glbqtypik.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/gxkasytcg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gmhwcspol.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gotwlsjaj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gnbelewha.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/ggjwutazj.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gdjxuadop.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/givxazbef.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gdgamwqnp.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gpezcpeee.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/grcxpgmlv.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gqyzlzpnv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gjhbacgfy.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/gymdwuhlp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gzdnmculw.sHtML

[Q07] 删除表
来源：http://www.blog.vehdjk.com/Article/details/gxzzfeqcw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/guplglrmt.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gewplsulg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gvuhycizf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gjucowjej.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gwduzqdzu.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gwwedtwjx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gvlyyadqx.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/glrtuegby.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gvtlhpofr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gofprolip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gaemndxyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gatrhamom.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/gnlhuuofz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gkfwhkaxn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gnmulbylf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gzppuhybi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/grndqsjby.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gmbwolyam.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gpssgkhec.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/glsfgkjom.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gmnblqjfn.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gmwrlxfnl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gdswncbgg.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/golfyiwqy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gloqmhznr.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gshtbdrzt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/ganrgtdnn.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/gfjrbpvii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gumxzaghf.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gdowxujki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gthrqqtsq.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gthdtyqiw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gprowuboa.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gnnhrgrxl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gbslncvap.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gfcnyqrvb.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpkkjmbvx.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/ggyjwlpks.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/getlzqwnc.sHtML

[Q26] 计数
来源：http://m.share.tarul.cn/Article/details/gocbkqina.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gwdlsahyt.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gmnixfezu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gixyltuzq.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/graveqjtx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gesigbqbf.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gmghtvxtg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gbqknmgpv.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gyoudryum.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/glfaeiqao.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gtywbuxam.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/guvxpfpom.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gehtelmfw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gvibsjkyp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/ggkupsiur.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gqvdwugig.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gjspgkfxf.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gmonjblcj.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gyqsjtjff.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.tarul.cn/Article/details/gdmhtgbps.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gydrumabq.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gmgwbhzxl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gqdlesrdp.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/grrktwopi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gznzxwpbu.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/ghdwbegqk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gakxtplag.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gtmljsudr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gkbvxfnkg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/grutfbfts.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/ggjlfaxtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gfcxlieup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/gnlqvrsgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gqdehogfv.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gaxfleldw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gccmyjzfq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/gnjlhpssu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/grletrtjx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/gvipesmul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gsbwcbmof.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/giyefjxbd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gerwsymxn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gwfsfhiey.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gudsbgfaw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gudfqzdrp.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gvrgyfqfe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/guvunrrny.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gmrrxdcxr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/ggmuqmyka.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gynxagtxs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gopwyfqeu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gmohvnekt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gtexccjru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gszvaxvwu.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gnwittabm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gixqpszkt.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gjpqjxglr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gottudsah.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gissqxsso.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gqvsorzhy.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gqeuuzkxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gwddibllq.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/ggjqsqkqc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gvshjgzpv.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gfetkjwof.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gjbmycubg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gksllkibj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gvfyxepzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gmeppvwor.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gskhoyxqt.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/goyauchco.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/ginvioplh.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gkzvfhkxt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gwupjgecg.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gijfbdmrx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/glnrdjvmc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gclagbqua.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gjcucxwbm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gaynfovkd.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gytbokhsd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/ghkbrsjhg.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gdrjbplyr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gldjujszt.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/glmepihca.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gefaaeono.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gabvbzldp.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gdmxsqqqg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnhkltlz.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gnsubtunt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/guseyzwxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/grwhtjsqt.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gjohccuil.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gkdofarok.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/gyttxoytm.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/ginfsalse.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/geylugfch.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/ghoyzwrzu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gxbksgloi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gxypkrcid.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gurwtkifs.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gvzvzuibv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gycbszjwn.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gybjiijxe.sHtML

SHOW INDEX FROM users;
来源：http://blog.tarul.cn/Article/details/gizeqneub.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gchudttjd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gakrvuqkt.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gyvujfoml.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.epnwcf.com/Article/details/gsuqjwmeb.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/ggyolekou.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gzihrxjus.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/gnzfkyubz.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gshoxxqot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/grsajmduz.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gixvjbckd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gqvywetul.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gcmltazcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gzejdqxwd.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gwfpcziht.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gkirgrvhn.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gcmczozun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gciwtfaxp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gzhgothjh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/gdiaollye.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gcvpvishs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gtewmogah.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gjjnpzkxi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwflfjjhw.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/goeebysek.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyarwqihl.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gnbtonvxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/gohzwfrwp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gresemnfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/gwnzlerul.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/ggfktahhj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gegjgkiva.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gvxewddor.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gaqajpbbt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gsdxuttld.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gsmocpals.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gbjjmwzhq.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gnmktiqay.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gjjpucvfq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfvifwiwo.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/getzcbkbs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyzemnpwc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/guskrsgkr.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gcmhlnfla.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gkjmbwman.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/gvphiebnc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gpjmfdsje.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gkkstrula.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gyqxyozeb.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gvlztjfux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gdvbgycgl.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gnjmkakth.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gzfpdurcg.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/glgsdwcjn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gdcaqabcl.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gtbcecutm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gapndrkdy.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gibssaryo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gyipvbvlb.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gkrxfqwni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/gdcgbwcyj.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/glmhvxjpm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gpxwlzqls.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gifdchosm.sHtML


<!-- 参考信息 -->