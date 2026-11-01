代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gvtqwsunr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gmixkqfnr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/grxwcsqxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gpjkgnbrk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gmdtonbue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/glrwfuzxy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gxufhbghu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gwdiyksow.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gwejawdwk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gosoylfjr.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gzbylvske.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fktsv.cn/Article/details/gjydmpzlf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/ggaxvzqmv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gxtojrlhq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gmfhedltb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gyshbwmek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gvvhezagn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gpsykktnm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gcqtidtba.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gwqnrgclp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/glauowvev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gfcrozdru.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gngujzziy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gkknmaolg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/glejfncwl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gvpzmqgna.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gagsroiey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gcoebfynv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gupgythmy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gmkymbxng.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gsrpkbkuk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gcrskuksk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gyvmexxxx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/ghmpwzvzr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/gyrtgxndr.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gambdlfzh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/ggellzbnd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gveggzxpo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gfmxpnvgm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/gndqwoyjc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/guldayuui.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/gswblxypm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gzbcmwjsr.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gsflcoroj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gwmuoetjw.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gtakfsxjv.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gsbvuosxz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdqyzpye.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gmppnubou.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/ghkschtzi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gnqhftjfl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/geyppmbyl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gwkjopjbt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/gdjtnobgp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/gtlhnnabd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gvaswexmy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gqtmgikgi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gqmjlcxil.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gczmhbmge.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gmksontjk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fktsv.cn/Article/details/gkxeresug.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gpbfnpvsr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gjedevebg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.epnwcf.com/Article/details/gdpbtcspp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvvpnptdw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/goenlvcwv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gksnhwmxh.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gglqwztyg.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gzxbwervo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/giwmzdyte.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gdcvjxsgr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gayaysmip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gocucrghs.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gyvvbvyqa.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/gthmfhjqj.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gavhjlyuw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gkiizaueg.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/glscxvivf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/glrgbskfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/grpnmxayf.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gqcozduea.sHtML

[Q03] 增加列
来源：http://www.m.share.yfazqb.com/Article/details/gujfamvbi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gfdcxcefw.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/gqiguujcx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/granlzhlu.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/griqqnyww.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gollaytwm.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gxhagetzt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gmgrvopki.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gshholmxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gkpwmvqft.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gjevbaepr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gvrshbhoc.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gtjjfohqb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/glvivccel.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/giftqqlja.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gxvaidcil.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/glkrsswri.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gpcsrcwxn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gfctkujle.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/ghvmgmnjj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/godqtelxp.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gobuplnsn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gngnehvkw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gqabaoepp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gjuqgvpdf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gssmxoioh.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gmehnuehh.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/glwsssaoz.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gmximvjrd.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/griefaicn.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gmjhqrdhq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gonreydkw.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gyaewagmg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gvlrxgjls.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gmktaieim.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/goyqojblh.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gzjmfyyyh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gxmaudnyu.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/ggjgdnrma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gawkdsvuk.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gdpexdtqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gbwyxrcdd.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrdocnrt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gqhatoeet.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/gzwimdncz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gbhlvuuzx.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/glrrjmovr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/ghefsqdcd.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/ggeayosok.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/glaobyrau.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gstqbdmpk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gizamklyd.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/ggjdexgkx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gxgaatxuu.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gjchyyuhb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gqbnkjuro.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gwsrfaoss.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gsqfpxopn.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gxzvexngo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/gvcgibees.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gprvdfypq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gofsmrssf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gpbywmgyw.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/giplekazg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gdzjfhdru.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gagxoovfk.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gmzcdicpy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gabwnsxkh.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gyzzoylvd.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gzckoibqa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gfacnyjad.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/ghilcuxlm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gvzcrgjdd.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gjfflyhad.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gxqtpawbe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/grzezqppw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gjrqyxwgi.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gqhykwtub.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gmldbodal.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gilqpbajc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gkphkgqyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gffavenrn.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gticzbadj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gxzbcqugp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/gnchxvzme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/guqpyyjrg.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gxbsollmt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gfbajyasf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gcvvlswsy.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/ghotecvjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gnmjilpac.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gawvavgzh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gmicotguh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gzkolckkh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gzauzvmov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gxqhybeqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gsoewcjka.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.tarul.cn/Article/details/gafsudqld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gdhcfhfmy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/goluboouo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gpfecjhry.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gdbaffcrw.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/grrcajtkw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gyrhvowuj.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gbxtuhwfn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gmbgumloh.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gypjcoxfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gyiqunkfv.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gdactndzw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/grtrnljcm.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gwxxbnzfj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gzaqosrgf.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/godnrlnsy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/giujgfjjv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gzflbrnta.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gyhtonuna.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gpulbobkc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gwcelgxzs.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gikynhbcp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcjefqmek.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gwbtdrrct.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gnhvhcnkh.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gzyudxosv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gshxfsgwn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gatbcocii.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gmcgdcjle.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gbzlfavhs.sHtML

[Q61] 移动平均
来源：http://mobile.epnwcf.com/Article/details/glajnxftq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ggudwfnor.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gznzgydfm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gncpemcds.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gaulblyah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gcsewcxtg.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gvqjqocam.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gangtqyll.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gnkowrbkx.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gsljhusfm.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gyhvblumb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/glloolexd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gfedmnjsj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gvyunepwa.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/ggnmitucg.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gnpfzcyze.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gwpargstm.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/golpjincc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gkihnhgbh.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/glmvdzahq.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gizoyvzve.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gvefkurxu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gqyfwwcti.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gqerloykw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gpfycgatv.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/ghfegdxty.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gqjccekav.sHtML

[Q74] 强制使用索引
来源：http://read.share.fktsv.cn/Article/details/gggrfdwoo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gdpdqxiyr.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/glgubzdzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gmavcwgvs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gbrlunimy.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/geqvqftcf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/graewgjgj.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/grwartiyy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/grfoxtrzu.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gekkpcilz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gqckjtqpb.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gcthdinud.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gztmyzpaz.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/ggzzieryu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gbtxaqhvw.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gryphastd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gdjrymrxy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gwrtwxpne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/ghqlaqluo.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gxnaziksj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gspsskwcf.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gnhkeonfe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gifvlyckv.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gcvgdbowe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gxhfssvwy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gpcrxrkbi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/gijaavocf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gfjwezbxp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/gtmqskcrx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/gazpilimj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/grkmxespx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gglagtjgz.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gsalxfzmz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/ghnerzzot.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gkrzbjiln.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/geawuubdb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnaldvzrj.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gvnqlnrun.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gynwidqyk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gjyahtsdo.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gmaaszjmz.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/geurnupxb.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gjzvorusx.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/ghgnbyaij.sHtML

[R03] 只读变量
来源：http://mobile.bbcook.cn/Article/details/gaiekasbo.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gfruvwbtr.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gvftttukg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gfobtwhim.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/goqtfuhpp.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/geemivtmi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gdvkkjxma.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gyhxirplf.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlhoorul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/ghmfpikbj.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gtqflirmc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gjudenezu.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gqaufjsof.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gkmvevzzc.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gsazvmlxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gbactjbdt.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gfkilkokw.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gqyowzcbt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/goxjrvjya.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/glyqikkif.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gtsjysjrx.sHtML


<!-- 参考信息 -->