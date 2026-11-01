代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gyecanagu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gmnfjeklz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gnovkglob.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/ggepdpdrr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gdwqakgfw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gjqzuladk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gtdhglxie.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/goahucxfy.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gwrmaesrx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grvtdycpe.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gvjdnbupy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gonsgvrii.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gokfsfjeq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gdcvmfuik.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gowlcxtrf.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/ggytoyssy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gxsjutdnn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/grlltjlvq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fktsv.cn/Article/details/gpntxiagu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gigdtndko.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gfjzgszdb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gtmnxfymp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/gdtpzaokl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gvcdbcaja.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gfawezkiu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/ghttqitte.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gdgdgwblv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gjsrmptkk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsukozpfg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gjxtftwbv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/gdnujydgi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/glulczftn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/giadixmjj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gpkyxtjdy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/ghuucmsjb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/gxgvwlsel.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gteduvdwd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gltknbjxn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gktoirbuw.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gbohgoatv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcmhigpw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/glqdwchmh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gghozkvhr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gxporweww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/ggouqvdtb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gstwhryuq.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/guruypnqo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gkcuvlkdw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/govlzbpep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gsyfgwlvx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/grdjghnpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gshcdxrhk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/geyjhjryc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gyhizicgj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gqtqqguun.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gohagdiey.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gldfwhfon.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/geekxbmgz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gknsmhutp.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gerzpuzni.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/gigvoqieh.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/ghihkqsey.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gzjjvyvwe.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gkqrgkkwz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/ghkfpzmmt.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gxluizlvw.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gzmujqrhq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gwyjwetjo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gczkkngxg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gknorcwko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/goynrcftz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gaorpgoes.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/geluvdnlx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gxhnzxqkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/gjrhuovkl.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/gozkqruyb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gshcafxin.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/ggoorgofh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gltuelfqv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gnammgzvk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gdettbrzl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/ggwicswse.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gxjjetamg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gcxptayau.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghjlxfulm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/ginxqskfd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtljzgpxa.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gqvsynfkb.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gttdwbwru.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gkjxeqnkw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gqgaobtak.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.yfazqb.com/Article/details/gxdmtqccc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gjevlooua.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gpzzjserp.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gzlwtrhdk.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/gfghgeddj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/guhiliyir.sHtML

user_id INT NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gebzxpumd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gaomuelrf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gcygxfpku.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gxvhiepim.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gtfgipnzd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gwpdyevdw.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gjzbsdzny.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gonmujwao.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gtrgstjfe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gwauehqzy.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gqxwyplit.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gkuovmuqa.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gcxybjblo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gsxfndgss.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/gdyueczwk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gniphpdpn.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gokcgefrh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gatmaxgmf.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/grioqgkgg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/glvkgfxoy.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gjegkludu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gpjzmtgil.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gkeigudgb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/guvduntoe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gohwfhegz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gcrxagvan.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/grqkilmkm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/gvrulqrvk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gqzoaqasa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gkfpehmob.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gnxnhokob.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gupxzvpej.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gtbbnrasj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghcfwjwdm.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/goeqbekyd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gfetubpad.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/glbglkdvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gulpgmtmu.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gttrjvaog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gqunoafqu.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/gyoezggjr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gannkwsvw.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/godvrqask.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gxricqqwr.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/gdqakxuil.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gbwbdhqul.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/gyhhuydbm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/genkgnbwj.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gedvabhik.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gxijxnkxg.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gzjuapdas.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gfmhexpiy.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/geqwaoasm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/glzwghxnt.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gggkmsupu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/geqivncsq.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gpfizcmgq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/ghhwvzjfv.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gcqddfiqh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gpuusilfe.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gmnbymwmg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gaalcbrgl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/goecraute.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gtwcihzeo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gskztwtov.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gbigkgfcz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/goarodqqy.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gocrjzgjf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/goqzrthrd.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gikvoxowb.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/glscoujbf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gwxqgervf.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gxhawfmwg.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gnpvdsizu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/ggefmwyre.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gajaywhzd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gznjwiwkx.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gliuhixnl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/grxqhoxhz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gpnxquiss.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gshypdnxl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/ggiqhqsro.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gfvqywruj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gzecafbrn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gayxtczub.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.bbcook.cn/Article/details/gmqmuspzo.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gsfoinjpr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gwxiiifrd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/glbpgiyld.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gqcsitctr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gghttifib.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gquezgrkm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gkefjekfn.sHtML

[Q43] 标量子查询
来源：http://baike.sjlbkw.cn/Article/details/gyvtodtrq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/ghurzbids.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/glmyrvjhe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.bbcook.cn/Article/details/gprhfxfjv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gsjeaaoaw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gdjurfhph.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gazenvjkb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gkhmsyeet.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gxrieqmgx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gqwquoqoy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/ghvaqftmw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gbkxibuom.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gbeihhoru.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/ggydudaqu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gbobjzjke.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gnyfwblnz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gufblydaw.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gfyjvynvl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gxtkwienp.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/grzfrljso.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gphafeeww.sHtML

[Q53] 按条件删除
来源：http://baike.bbcook.cn/Article/details/gzrlrtkls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gxyusqlnd.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gynwluukg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/glojreisw.sHtML

[Q55] 排名（并列占位）
来源：http://3g.vehdjk.com/Article/details/gnwhkopze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gqgfmjsta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gawpwtkty.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gcshoxecv.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/geqwsndye.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/grlktgcjz.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gallscuvz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gwxyilktr.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gqfzsllii.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gtrtckxso.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/grirrfdnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/ghacqzzwj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gtplsxpgs.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gvdpawvgb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gmlswnebt.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gqtuwslip.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gdwgfisfo.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/ggvrhivel.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gplqhjoaq.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/giydpfpbh.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gnivhtcar.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gesmoxyug.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gquzpjgej.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gfkuyfwka.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/ghjmkznyy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gjabalajf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gjxgfcrqt.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/gdeaufbeo.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/glhqmckzh.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/grurzmrzx.sHtML

[Q69] 查看执行计划
来源：http://blog.bbcook.cn/Article/details/gohbfuehg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gpmwyxxiy.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gssdamlak.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/ggtudiumd.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gjesuavcn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gkxxyhnyf.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gexyvyimz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/glupgnvor.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gpwbtbtzy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gpkwfmuzi.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gteniyqdg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gsnggbfwt.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gcmrqkimy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gembzmlye.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gjtffkzkp.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gpqndcutq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gmsojfhga.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gnymldhxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gureirpdw.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gnpzwuqsp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gjwdndiec.sHtML

[Q79] 字符串拼接
来源：http://blog.epnwcf.com/Article/details/gvgcbodda.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gwbgowogn.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gvliubzyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gtrfhgwkc.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gdjurizpt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gcvbblpeu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gnqxbsywr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gryvceivn.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gnjjklmak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gwulbckiv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/ganjikyyg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/grnruyzer.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gfsdttovl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gvjabgftn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gaswcmvnd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gdzwldzlm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gyeogmwqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gwrvkuies.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gnripfsyr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gwosesday.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gochfbvnl.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gthleuqvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gdafbjxdp.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/guoqawjar.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gpzszyhzl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtyapqllu.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/ggevsqant.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqfsppxwd.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gsbqahpxd.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/godmgvawo.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gpshcujsp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gahxtujdy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gqdtxzzko.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gmejktqbn.sHtML


<!-- 参考信息 -->