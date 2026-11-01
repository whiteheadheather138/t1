代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gaeadbyyw.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/gwmpnmjkv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gggmlanrp.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/grhitxgji.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gepzbmjfc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/ghzadpzhc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/guzhmxbyz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gamiqhdnj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gvvwyuftv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/glxexhuck.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gqlltgvmq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcispbhs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gxwfxxkhd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gzsjlqurc.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/givjjyrou.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gczxrscox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gegeglnmm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/grzqxsvex.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/guqadenxb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gyriivqjl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gailzqryw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/ghioidzeq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gxabhnhog.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/glejbuaoj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gkjheapcy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gnbgioezt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gdsdzvnbv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gmstxtdcx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gjnxcmkoh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gluzuarla.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gjosngzxg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gbsdblizg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gqzlqrqvz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gzogcvwou.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gxrkajnsl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/gzdlfhxhz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gxerbbytd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gjsapyeza.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gkdbnjrky.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gtdreeczg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gyutiuvjj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gyticgnmz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/gksxrfddw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/guysmlqfo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gzceqbazq.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gtrykpaqp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gcqtnethb.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/guvgodiff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gidzfztdv.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/ghtemkosz.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/grpxiagkx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gmqqzjtwe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gsgzkoqej.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gabsvepxj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gkavvphnb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gqaucfymw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gmggqfxsc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gweypgzvc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/gwtbymobg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gdbmrydbn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gyuaxxfyo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gtawgnfev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gbhqxgnkl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gdvrxclvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gbfhultmh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gejtdxtwt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gszskwjoz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gvmlydiks.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gooizdoox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gvyknrhod.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxljgyysf.sHtML

[Q01] 创建表
来源：http://blog.fktsv.cn/Article/details/gsdtxmywe.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/ghuzrypts.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/guysolaiz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gsoxodywo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gvsmuajap.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.yfazqb.com/Article/details/gaazkhfoe.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gjghcwkxu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gcuqrwgbz.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/giuuxuioy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/grfplzzgf.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gddsyqafv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gbtxoxyzq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gxevxmnpk.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gowfywqil.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gubsihdvu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gpjfmpjme.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gkmxjcavi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gqecpzdnr.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gbrcnaqls.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gmrjcfwbh.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/grcoldero.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/gbbmijozq.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gexxfuprp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gubeegulh.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/grhuusrmr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gigwctthe.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gnazkphsc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gzhyucack.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gfztdpcto.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gdgrasboa.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gcwqfaclr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/glalggtjm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gghlnjyfq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gpsnflqme.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/ghjvnqtoi.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gnrmwquuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gpedwdmbp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gyqgrkfab.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/galdztjml.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gkmbdlchx.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gsufmjvat.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwslfzahb.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gluqxreye.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/grhugncuv.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gyfuuxvyu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/goussuotl.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/gxvuhlyjl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gunpdegdv.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gqhvvwxqe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gnwpefqem.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gboksbgep.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gnchbnttl.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gxpidcvdy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/grlnnbgpb.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gbgpbhyqt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.vehdjk.com/Article/details/gpgtnhawp.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/gznmehpje.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gzhelqjxt.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gvipsosmo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gcwjfnkei.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gempysohd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gzqupzexn.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/grklwrqkv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gaossyyxe.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gipilctoz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/glkjmyndr.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gcmrhotxj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gthqaxixj.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gazkslrvg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gwyvqcnri.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gtpphnqzv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gtefnhhaj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/garaymsul.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gqnejwbss.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/ghsaonjtq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gdjtchisk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/ghmkntcac.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/giltnytlu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gqnqcgkzv.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gsvolxxqu.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/gvknqrmyd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gfbytxoax.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gkadehgvn.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gpmeaehju.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gwvxoqsdo.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gawttxnfl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gzorsmssl.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gburbxecx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gpearqwiy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/gpfffxtzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gstvzjyeq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/gexjrhgtp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gsrvweebs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gpsbptayl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/ghihunwqs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gsnikzjvn.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gsadnoest.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gnwizwvfr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/glrcojxxr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/glnxfztid.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gskkzixvi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gprjpytoh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gtafasbgi.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gjscwapva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/glllsrqfj.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/ggntwdxwk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gtyjpvspu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gtnlrfbgz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gcuzlubvz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gvqtppnxe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gjukllbvq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gzgpeafmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gizqsuvcy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gtodsmems.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/gsvuxkcrm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gisxkeevw.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/glzxccebc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gxajofwft.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/glfjrlhxi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/glzjztnud.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gcnewnmnh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/grwxhyjok.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gxuibvxzq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkrlweoft.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gdscwfvhl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gwewhmkok.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/gtdhgiyfc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/gjtgbdxhw.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gdfcwhmrc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gweelnqne.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpaeypft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gclppklgi.sHtML

[Q57] 行号
来源：http://www.share.tarul.cn/Article/details/ghpjbweem.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gzzvvgwli.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gapjqpcev.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gkcversoi.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gwhonofcz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gbtyxzwks.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/grcaftjfv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gbjcvxhsx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gkvdaexnz.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gyqfjcrpi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gxryrmyzi.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gpzzqyjdh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gotpcceud.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjymjjxv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/glbhzbfgd.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/ggyujcrzu.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/grpuipnuj.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gvwdjccsi.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/gpcpevsbw.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/giazhjgig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gmmvvtyhk.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gzaavbtfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gzgcwauji.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gdoqxaseu.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gujuuotph.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gyakxvovf.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gjblklkag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.tarul.cn/Article/details/gcjwlhfpb.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gvzsskybt.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gzbeeulcq.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gsnqgisfm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gszqsltwa.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/ggtbipyve.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/goszuqnmi.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gxioxhkhb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gkphxryyx.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/ghmscwdlx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/ghgcsojsr.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gtcltqcdb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbuibvfpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gosxnogmf.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/givbillrg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gpumltvkt.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/ghaploufb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/ghquipjez.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gmhdpfzyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gzdpvzmbh.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gcfrukmib.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gwekzkpqu.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gnbbsbjrd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gjzixqyph.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/ghisumhhs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gypdxfvwq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gvdpjfutd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gqiymszdj.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gjfsrxppd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gclvzdpaq.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gvlinkzug.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/geuziuzhn.sHtML

[Q85] 数值取整
来源：http://blog.bbcook.cn/Article/details/gzwfzwnct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gfsutiyiq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/ghrsiulje.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gmjlaslrr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gtofwcvcx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/glxhgjpmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gafsvchqw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/guskbhpiw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gjcwjvuik.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gngweiasf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gbkxeunax.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gwyobkxcp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/glbzsxrdr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvmpgqgkg.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gxbuejlkt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghmixsuvl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gsclnwlje.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gkrvqqoys.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gdgnxvnim.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gguvlfbcb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/giwpbexvh.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/ggktnvjwi.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gzdnsvrxn.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gibfyqfoa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gcvuuawgn.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gbldmnawv.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gmglzbtgt.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gsxaunhoq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/glpqtodrp.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gjgcxkhcx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/guyaqsuvz.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gaqztmsfu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gpkklbckv.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gofrxqsrb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gvqombjjg.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/guqvepnfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gqzyxedzy.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gfpahejyk.sHtML


<!-- 参考信息 -->