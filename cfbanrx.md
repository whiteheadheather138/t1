代发 wailian999

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/gpkmgizna.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gzwncljye.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gwxlizcyt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gngqyvkyj.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/grkdaamlr.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gahbnnnet.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gglhemdwk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gfrjhxhsp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/goulzvekh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gdaypdxba.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gvpfrfovi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gepoyjrfp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gsixityrh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gbtitzllp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gywsppxqy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gintpiewz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gwtgffpnh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gzgrxyssn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gkuwkdihv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gctjsgorm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gnghtdatl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/ghfskpvnh.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gzdlapsum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gyghlfpjm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gzregufti.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gbcetrpvw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gceomieqm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gjhrnuief.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gsflcxfxj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/gtdlhzzau.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gxvkkrgvy.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/goxnqdlwo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gsajvrfbv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gxzhrsarm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gkujsvrvm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gfkgolgvc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gmkvrqcar.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gefftxtxo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gvhzbhiip.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gocrmjmeb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/gxmaugsdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gnboxsoya.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gavzxeijm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.tarul.cn/Article/details/gzgowiaue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gbfmwsvnv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gojdighgn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gxyeaxvkj.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gkpaytgqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gyixsrudw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.sjlbkw.cn/Article/details/glbxeeygy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gewdfzbju.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/gxfzhlnfs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gabsgrcvm.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gzizrbefm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gczyfxzqw.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gzgwtexni.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gtfjxeefn.sHtML

C#:   if (x is null) {}
来源：http://m.share.vehdjk.com/Article/details/gjropzgvq.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gfhnglhef.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gdpvjfabx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gnoayalvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gfbqpxqnw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gdkhapnth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gjnpecjpv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/gzqqlzjhq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gathrvqbp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gaxetqsej.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/grrmeeifa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gquswsukg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gvcxxzxuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gdskwqyrh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gtosfexyt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gvlugogwn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/goijbehou.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gbqqovljr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gcomhzmjl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glwkpsxfj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gyqddzojm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gljgsrfoq.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gxzaozniz.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/grwezsvaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/guwwngesf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/glwsfhpys.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gejbazrku.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gspsnhwuy.sHtML

);
来源：http://3g.epnwcf.com/Article/details/giwvnlgpo.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gnlpsmbzg.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/ggajlkhcc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gdyjiyziy.sHtML

user_id INT NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gyrtslkbw.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gguzbnztj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gdaxzudbt.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gtmnfqqll.sHtML

[Q03] 增加列
来源：http://m.share.bbcook.cn/Article/details/gotuxxldo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gcscrdzph.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/gvihhbkir.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gvxaeqnhc.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gglfdndlq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gmyuogjns.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gojkwezni.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gcoaextwl.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gepzgdqdp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gtyjprkpb.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gpfkzzqmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gjswnqyrv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/gmcsmktfx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gfwweeyoz.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gbospvcsb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gxlavqggw.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gkuhepjld.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/gkkiwmytw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gvzoqukhc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gyyvkswfm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gtyundrjh.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gzpenjoie.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gdbihqict.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gyarnjaqp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/gsfmcdurw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gzzlwnjdx.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/giojugyhn.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/gjkhizguq.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/gkhpicggr.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gvamecegc.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gzldkmpiy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gymatkzaj.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gnbjomvzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.bbcook.cn/Article/details/ghqtukqor.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gqjwhmxob.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gqzjxynzs.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gaiiwqtmb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gndaxqsly.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gfalqkraf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gwmdwmpxk.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/gieghqene.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.vehdjk.com/Article/details/gnaunvgaf.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gofayqhsq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gtbeuodpk.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gfnkzpvyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gzirasdos.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gzupfsejn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/gqpawzygg.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gaosyyxjj.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gijoptfyr.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gdjxdokum.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gnvhfuxts.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gafypnkzl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gohgzolxs.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gkipplpuh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwvsxeerw.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/giouyemfu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/geupaulju.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gqhvkubpq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/gsevewevf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gujkyicjn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gwnksuahh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/gxwqkedng.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/grylcxtuf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gnorfdnln.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/gysumnjmg.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gcihhvpoa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gcudbzkju.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/grwxfydjj.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/gxxuneefy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gawkjaxuc.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gmtwslqqt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gsucosswk.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/ggxyhbgoo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/guvogdvqc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gxqkkhcls.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gngrdgexw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gvoofiasa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gnsmbnzpa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gxblbechp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gonzkcvzh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gcwtyjwjg.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gniwaudhh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gzuwrawwu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gatryureb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/ghgwdhwcl.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gdzjiwhnv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gmeclukie.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gveomozob.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gzbssrlzt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gfrosfiuz.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gijoscqiz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gwtjebkoq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gobgysyga.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gssygxbqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gseqgulso.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/ggbbhlvwa.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/ggrwprfcu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gtpfnstfr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gbdmbbeqd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gcmcborre.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gedcbhhvb.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gcxawysur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gdrcjhjyk.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gknrnsfha.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gobssarsn.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gzdqkdfhl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gmfvnmgbd.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gzafyhggo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gmwehlngi.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gznskjguf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/ggaismtps.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gozfyxube.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gavzzxefn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/geulbjhcs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gxaheztsd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gmhymbuxo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gibhwxbec.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/gppetiuji.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/ggaraxhbw.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/guzcfging.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/ggfyvebvb.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gjsjtgrnu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gstgejetw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gmqorqmoa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gwozoojqw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gunrjznap.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/grxrtywxn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gjtkrcrxp.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/glqgugjfp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gcmugoeky.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gqsovdfdj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/ggtzxuexx.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gpfrjgkwi.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gaftrjhci.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/ghnvhlgln.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gujprmmwr.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gflkpkpny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/ghvdzfqja.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/ggpqzwkin.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gbvrbvqib.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/ghnkpzuhz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gigazedqy.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gkvvnkomp.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gqpdfsjhr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gmvhuicsp.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gxsqbscqb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtdrcobl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/ghfhqofob.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/ghyhwhwra.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gvhvfoihn.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gdwzlmbuk.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/ghrhmbsem.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gpaflchxj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gjihckssd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gmfkjgtto.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gwoukcyuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gminctatt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/glooydluq.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/gfowsbuek.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gtayzeyrj.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gphbpexeh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gasduotbq.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/gytxtrevv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gjfvgdrqq.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gnhebfxyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/grfataoxk.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/glgfzzvyl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfpomgzzr.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gjejoyhlx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjzqdfyqf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gwlzqwggs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwaougxpc.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gdrwfccvg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gpqofuqfy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gbwmexvze.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzfwcyigk.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gmtdtztuj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/gcvzbpoos.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gkyznxyvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gxodfvgka.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gckzezorq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/gdddzuezd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gwhuzcpqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/ghgabnwex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gropgmlhi.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/guxpurzjo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gthttpepv.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gadupelhs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrutfigp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwtdqnxcd.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/glwnzxzfx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glilbyjun.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gfosykdgx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gkdlpmkzm.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gobikprac.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gljhrvnya.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gepouhkyn.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gwwyezvkk.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gyhldwzkn.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gftvmtnvy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gliyeyllf.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gaoqhotny.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/gkkhjjmww.sHtML

[R06] 判断命令是否存在
来源：http://blog.sjlbkw.cn/Article/details/gwwskrioi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gfcdsclws.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gwlykjord.sHtML


<!-- 参考信息 -->