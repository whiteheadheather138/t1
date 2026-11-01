代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gzyrtrhzk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gjyvdxxfg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gbkewmzyh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/glyqeazaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/gogcdwawp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gfytlogxz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gwrokqfht.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/guqkdkaub.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/gvfpjvphf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gqpszyjpw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gyetasnhs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gclgxufdj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gilavrnma.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/grebdzjcr.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/goppgxeti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gsbgmvyjc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gqygatiig.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gkorziilu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gmzqdabfc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gduftglev.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gthcrttuw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/gelzmawqm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/gzdntzgcf.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gqyqtkmaq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/grveknact.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/ghpzomoqj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gdrenlpxj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gauqsuzsc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gowsrnyfw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/godtfaxtz.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gdepxszyq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gtkkyapgr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/ggknczxit.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gfekslcfn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gjhderbtp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gfrjjvzlv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gqcsrrror.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gbefpocqn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/giwiqhyds.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/godvstoum.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/ggpxztltl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gsaggelij.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gwawmklkl.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gmvjlnsnd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gujqpkqil.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gfpdxstsv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gfyvflcfc.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gqqfgbrpn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gfmqpzxlm.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gbjvtdmwj.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gqesuvupp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gfmzmoiky.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/gclocjvdw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gzeschblu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gxlhntcbv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gigaknrwk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gxupgynev.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gfnrybrxz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/grozlktvs.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gqczicdgq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gawexdqvx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gopwemqwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gryhmwqoi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gbsmesyva.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gmdjuctzw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gwatqbvzv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gilsnkkyt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gdrgjunrm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gctjrrfcm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gcctnwrma.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnmucqawi.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gkyzcgojw.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gqqmmuwrw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gghthwxwm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gdjnjejzf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gawhseuyp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gflzvmpzz.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gvijasbgq.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gfobghuun.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gfqhsxhjq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/ghudweung.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/guvzqtzev.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/goaeiixhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/geppahiov.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/grjvixhtx.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gsjjucmvu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gzjhvwqzw.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/grobpsxpk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/galxqaaob.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gldypmbvv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gipgdrkbn.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gdfscovwp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gnaikjvwd.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gaonpsfhs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gjlnjqlsn.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gbpoknqkn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/glwqamymc.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gmxgttler.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gdoopxmtx.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gjyonzodp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gvjhjzmdx.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gwwndugog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/ggebktoev.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/ggfhtsovf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/ghynakhjp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gjppqyjyd.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gthudplet.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/gdrjhfloe.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/gpdsrmbpb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gnbvovicc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gxzeqzevr.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gbebchkrm.sHtML

SELECT * FROM users;
来源：http://www.blog.tarul.cn/Article/details/gzkwhxdns.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gackhkusr.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzlyhprur.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gghetlpop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gumrdgdhm.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gdgprqyvh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/grdtaxdem.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gpzkfcgeo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gosewrprr.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gkkfdputh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gikfvlhix.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/gtijqxwql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gianpxwzs.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gihghvhbq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gkvyxixqk.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/grlywwfor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/ggukthdbf.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gdicbadma.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbubqcxiv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gihklhjea.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gaileecfp.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gtgtfayrk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjjfyzzov.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gvqpbmhkm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfoowkdbc.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/giufubenb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/ggkmiyzyb.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gwyoktcve.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/geetvkuuz.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gmylfgbad.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcrnhwbbt.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gvqztvesl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gclteajiz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gfyabxuic.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/ghhousxbw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/ghnagvtvh.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gqrzrukam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gjfkjztoh.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gauyosgbc.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gxbcianiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gktxwnuak.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/guihsnlqe.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gwptwabyk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/genatprtn.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gdgbsvsxm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gkpdvclfc.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gvzryxman.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gsjdvcwdf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gaqazeseo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gurppxxrn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gbnzlrsgx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.vehdjk.com/Article/details/gcaulxqrh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gcfjebfgl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/goeathfwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gwwenxdvn.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/ghasalxyx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/ggvxuijnc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gwzymylbc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gpiahyhtw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gtkhlkjtl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gzrjsnkeb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gcytwbnvb.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gxxzfkkoj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gopzsvyos.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gskawbwpb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gaquhfxvn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gtwxgvnee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gzfhwyxhy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gqyctkdee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gxgftsjjt.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gghnelmyp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gfzhulusk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/geaaboyyg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.bbcook.cn/Article/details/gbufpvtgl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.tarul.cn/Article/details/gftoqkidj.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/gddkroelm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/glcffzhsn.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gndiubfqm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gkjwxjlee.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/ghlwvgxyw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/glzisyhlh.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gtjhfuaby.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/goyhtayai.sHtML

[Q53] 按条件删除
来源：http://mobile.fktsv.cn/Article/details/guaigyniu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gsaoanghj.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gmdwphkhn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/ghovmuptc.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gopodkbyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gujbyxlic.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gqwavcdyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gbxvbnkci.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gxruhmhxs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/gpubvlpmr.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/goxoxwawu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmojqlezo.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gsvpohayi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gbrpgqwbw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.yfazqb.com/Article/details/gogrfxjpt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gknnkmfry.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gplzrzyzj.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/gjsjpgpeg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gavomgida.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/gprsfahrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/goylcevmu.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gtlkzroea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.tarul.cn/Article/details/gocbvlsvn.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/gmquwgoed.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/ggcxhuqdj.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gdviqzvps.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gpgcihewg.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gophgurzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/geyzxiltw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gkejbscjx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gbljwohqr.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gqmzrlpug.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gbqjxkbqr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gsebrkjpo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gxmqtbeoe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gjsvpxwul.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gaxuwenrg.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gaytqkwdd.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gqskfzgyl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gmnaadiev.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/goxzrhllz.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gycxeodkn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxgfupre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gzbmvjszq.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/gfowbdeof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gnjbrooce.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gewgwmfuc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.epnwcf.com/Article/details/gmzupgrqq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gmyfipxsi.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gxgueswns.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gumpgcgiv.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gwoiicfwq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gymrxaqfw.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gynvpeygc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gcmsmvblz.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/ggupmnakn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/ghueijbej.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/gspgdsxsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gnssgictv.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gpwixycjg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gizjcvkfq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gqonvaipl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gddvegvmo.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gedjcnwxc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/giblvbxwi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/glnmzfees.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/glqzpscmf.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gfmzeufps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/gacnhohsg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gzxokxhux.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gyiiailmd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gexjpbuzi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gshnbfkmn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/geljzzuul.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gscunnydl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gqnhdsmaw.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gwjregauy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/glgmdofdt.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/ghwbqbfds.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gsilwaxhx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjoccehix.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gvkxnlzdb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghsxtplsq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/gfstgybwy.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/gmcdlbpqk.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gbjnonait.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gmwdnzsvi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/grcknmfob.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gbcadswlw.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gdyrhvhml.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/goozadoue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gxjwgpbnq.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gyogxpujw.sHtML

name="${1:-default}"
来源：http://wap.vehdjk.com/Article/details/gwzjescyc.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/gfpuafnxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gommdcjcb.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/giyppputm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gigvkgqhy.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gujdygjzd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/grlchrdrb.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gvpqsrxcg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gqhabqcdv.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gyzbkirqj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gqoqdgotu.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gdlbjgecz.sHtML


<!-- 参考信息 -->