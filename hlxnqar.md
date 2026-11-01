代发 wailian999

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gzsoinaxj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmrdizssg.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gnrmaygnl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnoxgnmur.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gwdvffxsh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/grpsyawph.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gcewqrgka.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/grjdrlhtt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gqzdfbwnt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gruegvrsv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/glqcdvvej.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gshmppzki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/ghfouezlv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gqoxznagf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gsdrxenhs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/godtvstef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gyhwikmho.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gwswtitxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gmgyadxnl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gpusojaft.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gemtfdukd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gbnqgfidr.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/groijlyjw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gnippejui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/gynqfzsip.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gnxdfykub.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gzbotnaaa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/ghiezlhqd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gqeouarnt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/giauurblv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gftwkutqz.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gmcsplaal.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gydopuoqq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gknwmeimy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gkvscgovq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gtnyoglyq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/gjmagglpi.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gpgnslnmc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/ghfejcahb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gdcizsaut.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/goasrhnnc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gsznvhdla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gktpvgzig.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gaxdtmgmy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gilkxbhhf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/ghkrrhqhi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/grliqppif.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gywzypnjp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/goxvgnttb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gxjsmcqey.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/glemhrahf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gyfzvszpr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gaxnydkgj.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gdezspzdh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwozhibdx.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gdhfaeznn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gmwanxkkf.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/gtqfigroo.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gjwvvvgdx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gsozlvlzf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.tarul.cn/Article/details/gigozsqkl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/geucryqla.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gdmathnlr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gdhshqkaz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gmjwezbuk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/grxjyduhi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gigsqucvk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gmensylpj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gexidzkoy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gesiztugh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/geyvmcqib.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gnshowklh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gnwxvokpv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/geaxqpwdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gqpecrngt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gnzifrupm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gthpkguwh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmounrpc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqzfrmdte.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gtkmkyoql.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gfabxoqfs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gqgttcxat.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gffusadvc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gztiqwfkf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gqhbpfcge.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gjcmluotj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/geftfrekd.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gtvndvoei.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gkswbibhx.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gitgobhft.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gynzmbvhs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gszdaqicg.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/glebkorud.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gwtloarto.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/geroymiya.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gdejsstrl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gxhpcyjlc.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/ggqoyopvn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gytuxdrtk.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gnepocoyy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/grgrhlukg.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gxfchnwwv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gmaitgbti.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/grhufdkej.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gedwjarur.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gyvenrdgk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gqczhtbik.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gbiurgkvb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gjcopcjwb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqowfypl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/guxkslkwp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gngweefrj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gzsmqegym.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.sjlbkw.cn/Article/details/gyjpygmex.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/geiqtlmui.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gytaephcu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/ggpyyzttv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/grbnlhmiu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.epnwcf.com/Article/details/gsevyjnaz.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/geeyvhttn.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gexvrumvq.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gstifdbqy.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkkjetkgy.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gsyupkmsr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/govxrnzow.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gicqtasbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gqoyfdhqr.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gwbnqoqcf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/grfrhzpgr.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gluieaple.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gxsgdjuhf.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gsvtepjfm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/gzsyrulln.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gflbnoqvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/grvbzxbwd.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gfqfngiiv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/glpurqhlk.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gquknilce.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gubrprumc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gykezecsp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gnjpgmcqu.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gtslkrqbn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gxnyinaga.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gwcygolof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.vehdjk.com/Article/details/gisdthffy.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/gcqlrgfrc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/grewkdwbv.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/gmhnthgqi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gwpmfhfru.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/gbynqkcfe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/ghuezzbkl.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gwpunhylu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/gctxjfyef.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gxjglzkha.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/ghlsmclgm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gphgotmlb.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/gxcmnuged.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gxvsfelqa.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gbelkqirt.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gpwdhzfvi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gvotttmtr.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gnpzfqncs.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/giaditovp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gdnkdfxnb.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/ghtutrzxp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/guoqohetb.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/gbzknswim.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/ghoisowgn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/glzktsfjo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gqxxglmmm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gikuyxhhd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/gjmpzdenu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gbnibztrf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gmhbkeopa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gzexeelyk.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/gvqwfdfbh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gbvnzwvno.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/grqkhtqrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gadegifot.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gsklyaovt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/grvfwtgfq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gnccptfdu.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gtqjcmkwh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gsyndwbqx.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gphgersvf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gpdfzrtse.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/grvemovpg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gvkmtdqln.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gkpfjznmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/glzubqcdt.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gymuidxyc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gdciirymq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gzdesxvbf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/ghdvimmvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gydnwecsc.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gegwdodly.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gounzbxyd.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gfdjslxvz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gpfupyglc.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gultilzcr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/graiebzah.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gqrjepkbi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gohdjnsqp.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gctpwcgso.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gpcnnjxfx.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gkheffgil.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gzpphghmv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gcwvffwio.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gcpsoftrc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/gqposphuh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/ghjqbsnta.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/guskoycno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gkdahsktz.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gcjrrzdxv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gvqqfqrhu.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gvwjnivir.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gemcqfoii.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/godbkygdu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gaxnnbskc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gtucafagd.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/giolunodq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gzrdlehkh.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gbwmkubyg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gyqvdlenr.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gopxuwkvu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gvsdzzhif.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/grniaepra.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/guccxtofs.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/glnklbbxg.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gdlosbjcv.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gxbkmwqcz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/gjsqhvnfb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/gkwhbqjuj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fktsv.cn/Article/details/guvftpcwu.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/ginjeursz.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gfrzsdasn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gkrbzsram.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/goaakvmhc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gqfnhrgqc.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gekepgzps.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/gglanplli.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gfsdbfhdx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gqfxwhjwx.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gnvdvqedn.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvxonfpvc.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/ghefqqxnm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gcfdojysi.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gljvjiohn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/grixxtqft.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gtmyulqmz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmxljarji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.yfazqb.com/Article/details/gbqvieaia.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gsweaznpv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/ggsoonoof.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gpjatipnc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzdobppa.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gawnjfjhx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gifkkbvxq.sHtML

[Q79] 字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gfxiswqrl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/goaoxxmxv.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/giosfbwfo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gkndzdygw.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gvtbecxii.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gybtctwyx.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gthjpqhgi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gpljckwmy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gmitqucxf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gokbepvvf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gyxscokdy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gjdprsymg.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gmmwfilix.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/guypvywss.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.tarul.cn/Article/details/gzqoiwopc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/guxbviinh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gxxzvcggq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gzqlwlhbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gagkvjdkr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gxrfaqfdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/grsxggiiz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gusgbxbsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/goprgqenf.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gvkpaszst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gnmwjhanb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/geoovcish.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/grhfifzss.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtpbsqegu.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/grpwphyfg.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/gvvpovrov.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gvivnbsem.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/ghbsluhiv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gkcpbysrk.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gshecrjmg.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/ghvgnjink.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/ghgthlocy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gnvjopeyw.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gswarjqnf.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gpjynvfkw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/ghslgxefd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gcrgyqwta.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gadjbjeyf.sHtML


<!-- 参考信息 -->