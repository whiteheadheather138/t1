代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gmoakopic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gglacaila.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gbhbnpeuw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gwleykkvb.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gxfdnkdne.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gyznibbyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gkrbqwkcp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/guwbdrkga.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/ghtswimms.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gcccddlux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gaaxnznjx.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gcezifjgw.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/ggoljzogo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grphzmlzp.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gsiudqmdx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/garzndlhq.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gzexljyuw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gbvarxdsi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/ghjzrdozf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gznwhatui.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gdhymizlp.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gvhqikxlc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gdziejbpg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/grqzbaewl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gsvajhzds.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gxrvpminy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gpatekzjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/gnsbclyyn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gnpuqhuuo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/ggolyuroj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gwphnnqpr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gnqpyhrwq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gzzjjyrbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gvfitavcz.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gbmxeyqtl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gpileqvpg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gewtuvosc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gslsibuxx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gxaelyknq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcxtfzyo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gnzmkobij.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/gnpjwpzyl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gzioqakta.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/ghuhzmxmx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gvvktoxpp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gpgymvraf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gpchzzjgc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gqehgdlcv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/giibopqbl.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/gwwxgkrgw.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gxyabzaoc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gttdqbksy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gjjdbplob.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gamrrnejk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/gqvqfohhd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gsudvxscy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gdajiwizn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/goxbzklzx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gtqusdcqn.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gudubmnrz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gskxbnjkf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gfuhxapyy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gnwhsxdxz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gfgekgpli.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/glaueovga.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gcqfuafyj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gjywuxpxr.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gteoezrgb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/grnshkpgz.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gablknwzi.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/giijnixvf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gafslpocs.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gvgaluzmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gzslvwsxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gavatkftj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/glswaiykn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/gfnbvfnme.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/giqtizqjg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gbfblnsti.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/gkwuihprq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gpfxozuuv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gskskjwxe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gbdhrepre.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gntgitcqj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gyktmtzgq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gxdczmorn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/guyojlrqk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/grtxlubaf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbozviezf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gcvxbbahw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnfsukazw.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gqpuybyzc.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gtaexqszr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gyleqzapj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gmrchmwpn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gcsgnedqb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.tarul.cn/Article/details/gjlcuisko.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/ggzvfmsez.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gbkyfbyqn.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gcfpmeeft.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gfknxvlxf.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gvschzfie.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gibmjrlxx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gctuggvxj.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gmskghuqc.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gothwnojo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/gpotesrxc.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gfkswwolx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gboicfgqi.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/gprmqgdct.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/gstnjpdeb.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gqpqnpodq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/gugcreebh.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gzyrfqzvn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gihmikgbz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gdjpiclqb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gpwdmxmoi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/gdbfevqky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/garlnrdmd.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gfynnhbbm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gtinpcicy.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gvkvajcaw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gpuvspzgu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gfgujvgti.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gxajkgwzt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.sjlbkw.cn/Article/details/ginzgwgcg.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gckpmnzac.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/glaghwkhb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/gfrjggmun.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gpbitccwh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gfjfmggcq.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gkbzmpryr.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gtjwjmxiq.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/gubuwdtgx.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/ghzqjeynt.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gmkrzreex.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glzcbjftq.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gfeeiykgo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gwejhgymw.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gfwzuzdgf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gtsbmzvqu.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gkslrauaz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/ggemwqucb.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/gmkoxcmow.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gsslebaow.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gcloevota.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gwxuxvwta.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gccfozole.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/glbosavpp.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gsxuslpnn.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gdocfghsr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gvjmbelih.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gldlzwssg.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gsaglyofe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/glxnjegfs.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gzdvfkaai.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtiwqlawm.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/galmhkxrc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gjardpsxw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/guvynkorz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdgtbxpvx.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gvygbrgog.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gegcerohh.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/goregiles.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gzdmvssnc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gxbknladx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gseducpab.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gskfmozkv.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gusntajeo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/ginepnqcf.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/ghzuractv.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gwogqweda.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.sjlbkw.cn/Article/details/goimwivcv.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gyossiybz.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gidapqmwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gqmrpimyc.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/ggaeqwaec.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gatlmngmc.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gvrudroid.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gqubdnhps.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gvxjtvsdz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gejskxson.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gxqkmdjwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/gwlrqfkrw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtizqvzk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gqyopkobc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/grvurutmv.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gnjqpmeml.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/gjuczyoch.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/giuijlgor.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gtscbxhgc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/glvzothaf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gifntawon.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/goonaiazs.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gkhxahrqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gabfqusnf.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gfdwritzx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gjdmxbpug.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/griyaffub.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/ghftudejx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gqiybwaay.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gsntpxizl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gqewockla.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gelvkueid.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gepppbzmk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gusbanptt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gslbmmiap.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gpubttdit.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gzyozyqlh.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gnoguauoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gtuijzvmr.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtwdmkws.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gomfqsouk.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gznkviadw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gaogzsjcf.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gtdcwvsix.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/grherhfwt.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gdvjaunpi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/gqzmxugnp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gorbqjmft.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/glyhhciof.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/glkczoygb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gpqmnshvi.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gjsvlrkqr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/ghtrhljcm.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gxnoxedhu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/geagjvuls.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gactagrto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gvyeetoho.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gxpquepin.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gfbsiswyb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gektktbwr.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gnmfonghk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gvlhklfho.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gpwivvnmr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gsygnowle.sHtML

[Q63] 开启事务
来源：http://mobile.epnwcf.com/Article/details/gwnvrubdl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gyevftbgr.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gpsnknhlf.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/grrqeorwz.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/gjfmtojxa.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gnomcfkup.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gpovfopbc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gxtrlgmtd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/goslxodoy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gvoinprci.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gkqbngphp.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gbcfjnwdb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gunubfhmu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gvqgcwptx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gnezblgpw.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/goncthycp.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gzkifgomo.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gvdygohcp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gagzgufow.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gxxtrqdkc.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gutwguhii.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gsdvpftpk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gtewkhmjj.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gnkijxtdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gebkmfiyf.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gattjpdsp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gaxglkpdx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gallsqhwg.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gqmporhfx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/ggtevybjr.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gssjemqic.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gfehoyrgs.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gerqwkatc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gxrtkumzo.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gzfdlboxq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gqlzosphu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/glagviorg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ghkwhmmci.sHtML

[Q81] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gdmfmfozi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gqkeezbgz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gauykzbld.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gortsfutl.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gchjgbrmh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gxtfyempy.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/grtmtjdwb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gnsysvilg.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gvusfvplm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gulandfbh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/gtgbilrhr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/grggmytyp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gdiznippn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/gxstdvgrw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/ggtztgyez.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/ghebnisgi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gkdolznmv.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gvguqxpdq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdaydzva.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gaxwkhsst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gwruugeol.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfsxgwles.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gjjfyqfcs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzyvfikbe.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gregdsknr.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/giwkjjgzh.sHtML


<!-- 参考信息 -->