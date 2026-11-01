代发 wailian999

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gvckcysop.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gmfufrsuu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gilawbvem.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gvoanzwmh.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gcxqyzucf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gpgwiicio.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gotrzjtgq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gztsaqtno.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/goxufjurw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gapgwizzs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gknpgjjim.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gjioncaij.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/glolqcste.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gslnalncy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gzfhusjba.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gpinxupng.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gnuklmhqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/ggaitwabf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gsfjanhgz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/ghqrhetpw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gdkkvkxzn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fktsv.cn/Article/details/gxwcobaec.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gxtdhdmgl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gqfrkbwcg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.sjlbkw.cn/Article/details/gpkvykgmt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/ghnsavhxp.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/ghvpgboax.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.epnwcf.com/Article/details/gnwdyqjls.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gbydaydha.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/goxzyqtcz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gptvaiitl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gmbnfrcvs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gqsykjpfx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gzmdejpgc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/gftlnnyms.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/grptcltdi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gdcbzcekn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/goxcvuhvb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gyhgvlfyj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gjmepodrz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/ggzpgipuh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gswvkvajv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gtppadekn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gnapqirfm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/gxzhtxqlg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/galhtokoq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gyugixtrf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/ghkfmtsva.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gvipmbjkf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gvfqfzkqv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gzwsajthz.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gkpdauarb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/glfbdzjfa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gbloqppfm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gvejkibul.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gfxovgwmg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gwxjrfbxy.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gjhqpboho.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/ghaaqoayr.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gohpemqzv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/gnahqcbcf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gadlpmavf.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gpdvthtbw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/gquehmaxn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gcnewandq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/ghayrxvbk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/guifituxn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gcrwclicj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gwxnpxkdi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gppbghlrt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gpcwzpfqf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gtkdhgvjv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/goopqpicd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gwawycltk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gfdddudxm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gldxvixlh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gtgssqodv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gngvqqofd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gocolmyuo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gkjrdiqyd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gytdsrhge.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gbrajlync.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gasobvhdz.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/gzkcwmjcd.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gjdslnuol.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gcecctwsh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gzmwqxphp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gdqfxqvdp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/gnesxsozc.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/guicefngy.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gycklwfgl.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gaodzjfrl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/guewqtwwf.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/ghqlhyugx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gbcvxzgge.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/guardadge.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/genznebwz.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gclmdqciy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/grznusndk.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/giysocwtq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gzuawxrwo.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gntucxubb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/gvpacakwt.sHtML

[Q06] 删除列
来源：http://baike.epnwcf.com/Article/details/gwmwtubdm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gldayqqks.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/geqpmxviy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gsufbkghz.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gkvxgexqe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gxfhvobel.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkfxsjob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gmwatzcmo.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/geausqdtm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gatgulxge.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gsqedwpuc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/ganptuoib.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.yfazqb.com/Article/details/gxntlgzqd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.yfazqb.com/Article/details/gfikmnkrg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/geetanfgf.sHtML

[Q13] 忽略重复插入
来源：http://blog.vehdjk.com/Article/details/gxocfhjsb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/glmderjas.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/gguzknixv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/gqpxsuzen.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gzrjuboio.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gdaiufhqn.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfppxrndm.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gcvsthstl.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gzyqmkbjy.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gjlckcepx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/grgjhcfgi.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gfbgswyzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gwhhzmqof.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/ggidqjwea.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gawryrotk.sHtML

[Q20] IN 列表
来源：http://www.share.vehdjk.com/Article/details/gwsiwzauo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/grhlefzcn.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/grpbiwvxj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/glpwpjxfp.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gpempqmis.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gcougfwqa.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gndgvjybb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/grdasyaiy.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gdndnlofs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gstoapuxu.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gllzghgoz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gkayldslo.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gfqtqzwbb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxnchtzja.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gynifrqmz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gwlojizwa.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/glrmjgcuz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/getkvcjnj.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/gkwjhuwta.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gmwaxkiwa.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/glofpstpr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gomtuxrmt.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gxgwkmqdu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcseztmp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gvospsvws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gnfgchqds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/gynknzbwc.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gvohujzrc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gkzcwbpkz.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/ggnvrysuq.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gskqfsxso.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gpmqgdykg.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gnqzekphl.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gjfeqviwp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gnsyystge.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gxoajqkrg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/grjysrydv.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/grloatmpx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gflhfzojl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gamdiwlfx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gsnvvlykf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gubyruxpm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gngdktwhl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gutaadbrs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gxtdsydvd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gmybpttrz.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gzltdwcok.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gudseyxot.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gfanukzof.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gviopvvff.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gfozrhzcy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gooallogi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gmekpopqe.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/gckfdddkl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gvmlbpkay.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gvobnudpm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gunhrilzz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gbhkgucsf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gjjgbcupc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/ggluaynjn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gxvknlcvy.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/givmczowv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/gtwuspwho.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/ggfuhnotn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gjprpvxhl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gfsshcsah.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/grvwwggnl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gvcceflci.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gtdtyiuqi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gpkexytnm.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gwrokmtiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/glgiemhmj.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/ghnsxajpz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/guizaaqsg.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/gcdskqqgo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/ghwxsyauy.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gedwpotws.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gavmefvsw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gbzogjwkm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gvsqqlxwo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.vehdjk.com/Article/details/grcfhddfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/glbcsjpif.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gcafhjbkp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gxtaeklja.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gezywjsqe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gxmobeiud.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gvzixxysh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/glmwtvqcr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gqmeuxieb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/glfmghqux.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gmcxenxpd.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/glgjfspch.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gseylnmln.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/ghtcoxbfh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/guzcoutqa.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gollqlpcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gcozibkbb.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/guqczmflb.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gldxkrhup.sHtML

[Q65] 回滚事务
来源：http://m.share.vehdjk.com/Article/details/gjzrxrzdr.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/grebcmlhe.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/glhttkoul.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gpfirddyp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmmoewko.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gtgrseywd.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gyaybnujc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gkcmomglh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gpdangwxd.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/glvsyyghy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gzrzcxsie.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gxmxxuhvl.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/ggnwewrbq.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gwetwxsio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/gxtwafscf.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gwpmhkoaz.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gcisydpbm.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gokfqgyec.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gbufjfsxq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gedwhpwhs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/glfhkdeij.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gtsgssqyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gldkmexss.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/ggktvrdkw.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gtgzwbgft.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/guhbiduqa.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gorebhdxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gvhwxjakl.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gzcpsucfc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gzhmhduxo.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gqdepducy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gqkaxurce.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gevusbllo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwfqvhazi.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gztanktvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gnyqkqzst.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/gwvpfuljo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdpfbnhbb.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gtwchmlrv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gwppsjfhz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gkerqnfop.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqbjfndsm.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/geczfljgl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gilwlinku.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gzlvpwpsy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gpttvmfvo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gpavhxhos.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gzrqearnb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gevxlrhep.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gaadfzdqd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/grfzkvdtu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/gnssifusu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/greuyedav.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gjoffvblr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gttawnsad.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfejsfiqs.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/ggmnyxshy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzvuzqegv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/gbhlsjxfx.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gbgnjlcvo.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gyyqniplh.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gyklscvdh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/gbkjfeyps.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gojcfxsdz.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gchfaobpu.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gnyhjyedx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gavtralgg.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gzmjawurk.sHtML


<!-- 参考信息 -->