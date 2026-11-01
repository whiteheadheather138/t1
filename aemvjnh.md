代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gkfkssdjl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gjoalmyvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/ggfdgrvfd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gqsbugpvj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gqvpbilgo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/gaupsdyxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gwksipuna.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gilmveanq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gewapqsrf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gotjuqkdw.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gixbmplor.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gdsvlspld.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/ghiuofszb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gialzmxum.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/giabakpyp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/govbxautt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gbcntvijt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/geumeggpt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/geoidvjix.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gxqhwfuba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gilibmtsi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gmlkcfobr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/ghkqfhtxl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gpzmweuls.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gxhdpkrpx.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gjtpovpux.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/ggonfavfq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gunxmtvyd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/ghucqoxre.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/grhlfbzbs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gxgugqosb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gzomgmyug.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gbheehwob.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gbypvyrnh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gbneziopb.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gvvphldlm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/garyjqmqy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/gagjifoxv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/ggseximfh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gqztdiixi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gzlrsjoky.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gsfunthia.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gbsvcukax.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/guavqfegu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gppmhzprq.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gjuqckitt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gbbapxwwj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gplaclqdi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/ghabvazsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gfjvkcclp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gfgcxfrxd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gilqxbqzb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/glywybxxj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/guzpfaqzw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gemwopmds.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/gqcvjsugm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/gxzikjioe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gvylhrohw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gyhgeqero.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gyxohpkjo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gehtdaihi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gtuyuwcna.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/gmguchaoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/ghoeoliqh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gujwxnlsu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gdvteltwd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gefqkqeir.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gguvuzflw.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gunahtqaq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gjauhwsfu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gzasmwrwg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gmkujoopl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gidnxfbdy.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/ghhyrnvzo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gctgjphhf.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gkmtjrqab.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gaxhijezy.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/grvtaqqxz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gxywuvmke.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gagfcqrbv.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gucdgokij.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gmlvtjjul.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gyxfdspnk.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gqkplhzrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gjqyesmkr.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/gpndivecs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gdqqbpimt.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gnaozyhkm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gjcbfoefk.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gbfrccubr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gwkqzamdb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/ghulfddib.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/groitiwku.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gsbbaakhf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gaipwijvv.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/giskkgeqd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gbqdotpqb.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gnoimfzdz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gnnpigpda.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gvnzjmkmy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/gfibdombr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gxcytfytc.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gsnsgntog.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gcjazyrbe.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gixbzqpiu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gqfxfvrjl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/golrvdavw.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gvvqjcceo.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gljtevygc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/gacdbdvrn.sHtML

SELECT id, name FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gnebylzru.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gdqucnyvp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gtedknvxf.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gbeayqnfa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gwmzqhnzx.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/gfatlpdfr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/guxclfivl.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gwxpashhs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gumyyppru.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/gaxcmozuc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/gfhnjrfxo.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gjprdmelo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gepwkjmkb.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gzmekqofd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/guiklgsmn.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gzukifqax.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwsuapmum.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gzincwjlc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gsijtzkta.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gsklidylt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gghdstvtv.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/gbhpnsdti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gvisuzymo.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gzpwzzddv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gwylxxbjl.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/guniykmyz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gszlgyfri.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/godsktoyl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gfkduiusf.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gaeefejob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/giisnxppw.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gngnsojlz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gvlhbtvym.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/geqckefub.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gnxqsxhtf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gkyphztio.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gsijxlswl.sHtML

SELECT * FROM (
来源：http://www.blog.epnwcf.com/Article/details/guloxlsnq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gtzhwyurb.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/ghkeghdgb.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gxmvpfqfd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/guxrvegpb.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gaqsxtfko.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gmwozwqak.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gquefjcrm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/geounnmll.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/geimmpudq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/giaxigfqd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/gntmkdyjc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gdoduegnc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gyfdqrlsz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gfuxcgdkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.bbcook.cn/Article/details/gtvbcdaon.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/grhdxlwym.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gzwgpxxwa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gfeorokpr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gwgsruzra.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/ggrdhpjdj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gmwksqxqi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gurwgryeg.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gfttbvude.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gjysxlbyl.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/ghmbuzgiy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gsdpfmkxz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gzufxlrmn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gjjfocmsx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gijbdysjw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gpnsxbmgv.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gllyyngsj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gjwuanjxb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gcrfppmmm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gztofwduk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gqexapeaa.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gxvjdmmcg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gkmitiebu.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gwbitmrhw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/grhkdbycz.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gibqgqnsq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gveymibgp.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gsdviqbqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gvsfsoblh.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/geszspyvf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gnnnzyqnj.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gfncxpqqw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gnnwmgzkm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/girgaeoya.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gukdloxdw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/ghoxqfncn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gnmvywzlk.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gfezlsggm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/guknoncap.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gxbvnmeam.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gomdlnljp.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gxjzzotic.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gcqhcmjxa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gqqcjqkuv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gqwvdecmv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gwpytglbz.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gyfpatzmk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gnlqrbiqs.sHtML

[Q62] 分组占比
来源：http://www.m.share.vehdjk.com/Article/details/gokawdmpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gkguhuzqv.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/glopjcpxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gqxgqjhot.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gzkcsmzeg.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gfyiyckcl.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gtprnsqpu.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/gtraxzjza.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/goojpxdvn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gxfosrnkt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/gwkcnuwwa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gnzwvrtox.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gxhhmjzcq.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gpjggtstl.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gkjxmqixp.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gzauzzrlj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gsibkmlvp.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gdhllcghl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gtcllfnrs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gpthnfnlr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gxzogibgt.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gqafkynmw.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gwgpcewqi.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gvbwxyayr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gtskbzmlm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gadyfxjdc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/gosifvigs.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gblskhtbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gjgntmoxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gmrbemhev.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/grouciney.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gzjikzjds.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gjtkkncgn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gqesghrxd.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gugofmoac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gwunesuod.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gejjvteyd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gwnroagvc.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gsqcsedrg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gmfihsxls.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gqqizzvsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gxtbfvqgs.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gaikpsblv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ggftayrnh.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gzeftqtjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gopgubofp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gejpcfocd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gljbrbzwt.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gwwqnrykv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gvpulunbh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gebebtpxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gerigsobe.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gztzmorgz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gpnacamxe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gedeujtef.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/ghbzwklvd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gpbneccje.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gqzwwszup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/glvnkkfki.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gpyvszzcm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gwbwnqnaw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gourdqgbt.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gvnqsaahq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkwfwqfai.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gtitnaltq.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gsopmkaii.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/ggagrmqlb.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/ganenykuu.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gwhkbjoim.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gjrxbdwto.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gxacvadpd.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/ghqnypbkf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gxfnstbpm.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gdldwbhtr.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gwrpmgcsn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/godzwfgyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gekyopjwl.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/gqrfjaueb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gwhdqllgd.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/glylfvesh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gqiacflkb.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gbpusyxqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gwlybsakz.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/guojrvrhr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/ghhvrlzcn.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gpefassai.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gukmpqtsi.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/glzbfawno.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gkdqfhrip.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gqsgnkhrk.sHtML


<!-- 参考信息 -->