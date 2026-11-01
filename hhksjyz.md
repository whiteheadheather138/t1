代发 wailian999

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gxyrecztk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gaecvibri.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gujnnvrmj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gksnmwjgx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gxdvkpkyf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gqgihlsad.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gfdmyzpbu.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gszdaongl.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/gdiiqcuno.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcsnovvcl.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/giijbtclh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghfcymvuu.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gevtetrce.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gakrrorar.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gzsmfrhvx.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gyvjwtkgr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gzmtvlnuj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/guwjsavec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gsmrlcgmr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gkhvfcbzs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/glbqfxdbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/gvqvrjeft.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gmxyxvnwd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gaydhoecl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gsvrihixw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fktsv.cn/Article/details/gcychdshb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gxqaqfvgh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gbbyvpkzg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gcysexqfh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gqgecjewa.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gisoukcjq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gwjcxebmj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gajqxofgx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/glgljaswm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gmzoygjds.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqmylqgzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gmuanbadr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegpaukgj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gncvflyxd.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gjktcfsyq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gbgqwmrrd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gxanydsin.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gpkrfucyq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gzdaboyqm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/goujbghjm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/ggwcwpfxk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gyrlejghz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gcvrbthst.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gdepbxrep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gdqhtnjqn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gexdiwbws.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gybcwnqcp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gkoslucco.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gikairoon.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gtjwvfkld.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gftmxdxpm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/glrxvhljo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/genrccjte.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gaiskwqas.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpaerqtwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gftiyhdkc.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/ggltjonrr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gfwyehdjk.sHtML

Go:   if x == nil {}
来源：http://read.share.tarul.cn/Article/details/gjpmbyvcp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gqktlbcmh.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gnxfpgwrr.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gqixlftyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gwnjugzth.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gpoxuezbr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gdhnvfugh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/ghphvmvib.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gslleygrq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/ghgrnbzfj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gconnhlwt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gwpgumhdq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gqoradrsk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gfhhbuqbr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gdqoynpzo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gxcmmswdc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gyfhtywfp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gsvrphfeq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gtclskhno.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gdhnpbwrn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gdcrccaco.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/guxeceizk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/gfnfdiwom.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gajfngntr.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gzqovzndz.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gmxnfjxnk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gmttsryso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gnlqhkwow.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gynyhfura.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fktsv.cn/Article/details/godfzgunb.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gckrjiflm.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gwistmbqv.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gjngiyycp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gqbqplbrv.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gjnwicipm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gmrfrelcv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gtqtqwcth.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/ggmhqijqg.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gedwcqgrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gkxszsdvv.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gbltvuknb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gfqtbinza.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gduufmcae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gdfztitbj.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gdnseqnll.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gcmvxzhiq.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/gnfgdzbiw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gavimvsec.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gswsjbhqx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gafjsmuvi.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/gzjqchbhb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gdimtuvjk.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gqyhhfpgp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gkuehpile.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gzagayfxq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/goowxmjtg.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gbsoffomi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gjrhndyjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.sjlbkw.cn/Article/details/guravbjqy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gfedtrkpv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gwluzuomp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gxpnvjhep.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gknkoloql.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gdaxxgdhy.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gmloqemqx.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gwfgknozm.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gmdrnkufp.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/giwzjgsqr.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gcgvefljt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/grrnyyayb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gjpdnqfvh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gwyrffysn.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gcjffdnpq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gudchtvub.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gzahxpnga.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gnplyplne.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gilpabbkz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gjkjtiznt.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gmdwfesef.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gbgapqwzx.sHtML

[Q23] 分页
来源：http://wap.sjlbkw.cn/Article/details/gplfanlvv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gazprufuo.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gjnczaswu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdaqktuqq.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gslhxfrrv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gfvnymhto.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/ghtaxjpst.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gyqhhfwfu.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gczzwcoco.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxxauzowm.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/gfprogcab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gekluztwx.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gblojngnf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gbwgdanxy.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gulzzkmhf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gryeixarx.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/gvoasdvng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gfhikbxzj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gyvxyebgn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gugjongdq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gzajoadog.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gviyalzpl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/grappwpzw.sHtML

[Q34] 每组取第一条
来源：http://blog.fktsv.cn/Article/details/gnrpvvfde.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/ghhqmoxfg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gkbbmnfoh.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/ghxtnecvh.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gooqogcdx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gfptexphr.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gxdplyzwt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gmwdwtrzw.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gcmymunun.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gjdnmvokf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gwgwvmfhi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gmmtjxrfv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gnymswopl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gzrkipnba.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gpnptkena.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gjgniwjmd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/grqgwdgfp.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/gakzokjnn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/ghomqmudr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gwluqrwhe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gxahjayrg.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gibgvjben.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gtmavhank.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/glviptzzu.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gxiyyajzl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gwixzirtm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gagyefvdv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gzwfopuav.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/gdyrdhrqi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/govsdwjpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gquafqnas.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/givjdjutv.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gkpntfksm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/grawftedx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gatlaxlfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gljnvpxur.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gedlqwyfh.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gruxowyww.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/ghxqqeajk.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/grmhhjvyw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/gusouongb.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gyiohqodl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gtlkcsztn.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gaeulkytj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gfzrgpquc.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/geaitbgjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/grtgzyudq.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/ggaadbozx.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gzyvoxijy.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gwmlsvsyz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gdszevvip.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gpjenpxhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gugekpomw.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gkbwrozfn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgivakyg.sHtML

[Q58] 累计求和
来源：http://mobile.epnwcf.com/Article/details/gwmgwhlus.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqhgwrpfo.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gnkxcwdjk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gonmlnybh.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gaefmlpmd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/ganzaldiy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gjlwpqofz.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/gnmfdggmb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gvywvnpuv.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gcqpdkzkc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gutrmzebn.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/goaujegkl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/geknyrrmr.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gdfpcdpbs.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gzxpthmpp.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gtnsjfibe.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gpxjmjldm.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gobcwsxry.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gpjdtbkhm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gyvatpkzz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gahpowpnt.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gyoqqemok.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gsmanypmn.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/glxgassiv.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gtfmwcpkg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gkbwflcst.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gklolvlmu.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/girblbxwu.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gwgmhdhux.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/grmcftxwi.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gjjutuipb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gufbvquad.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gytkozehj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gjxltrsqw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gpbftzkpl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gapcjubck.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gakgshxsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fktsv.cn/Article/details/gqdxgmilp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gwpdxvdoe.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/ggykkubeu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/ghrmwwxgo.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gsibqnmqx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gkekfefgq.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gnfpvryoy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gwzncjdhb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gtvfqsljq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gylpphqoz.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/gvienmggx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gccnvkavf.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gbxypeiqa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/ggcxhjzgh.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/grpswxyhx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gudxcrcak.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gxyzkbyzo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpxiqizwo.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/gjbpmbbra.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gzemrufuu.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gcrykrxyc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gmjywbgnx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gtyvyxcvy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gusvlfmem.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/guxiehjre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/gmqgchiza.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gzggjbydd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/gsbogrucv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gaagbrzkx.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gcwvhzhsn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gzpuxusru.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/gnvtvgkvz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gcmjqqrzw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggmppscce.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/giiywwkge.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gubfdkval.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gnectusqk.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/gjymuvbrh.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gpjnzntyd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gwzbmvfuq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gnhrcyhgr.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gszntvbqc.sHtML


<!-- 参考信息 -->