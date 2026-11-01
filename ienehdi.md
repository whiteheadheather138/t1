代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gcyhtqjix.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gtqkghjif.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gzlyzknro.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gjlwtdodm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/gwkaivtek.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/ggjkkkgyi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gojkqrvaf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gnnwtbrif.sHtML

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gwdvwgffa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gspcnodtq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gupbjxfag.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gkmhohtrj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gxbjxxsdx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/gmsnvtsae.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gtfhaxqyz.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/glkypfceb.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gmefndsch.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtvckyphr.sHtML

P. 常用工具函数
来源：http://www.blog.vehdjk.com/Article/details/gwggcaodb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnjlzgltz.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gxycykhdb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gqyqypysf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gzwycetmx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gmptaqbcb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/ggvjepyxq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gnhyfjylm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gcztyaxov.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gtjfwaoqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gfqyresrz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gjpnhtaso.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gkzsksbqf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.yfazqb.com/Article/details/gbalkhlcg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gofwsufrk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gsybuktdr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gcxijagtt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/ghcbukozy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/gcszgmjxp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gznibyxja.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gqeibqpsu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gamrdjcqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gkwskgjlw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gttelxmpc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/grkbnwwbx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/giyuxwees.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ghxurkwtx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgvaevrb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gekepriae.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gnxbzmfbl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gnrcockam.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gvhyrbxry.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gnmvltfqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/gduvngsax.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/ggqfyrcqt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.tarul.cn/Article/details/gpazpwzks.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gbrjotxrz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gosspkbgq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gndfbjlou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.epnwcf.com/Article/details/gsthwklsr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gfaxsvpyy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.vehdjk.com/Article/details/gsktatsvx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gmvjghbbn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gsmympypr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gydjwkcns.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gzrorfouc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/gnkvqzanr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gwdjhzovv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gxxozstmi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzatymdgu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gdasfvafp.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gtfionrsa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmnqzoyif.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gyjnlvxzi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gqdnfgbdm.sHtML

C#:   if (x is null) {}
来源：http://mobile.yfazqb.com/Article/details/gtvaafcwr.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/gvwkafura.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gblonrnso.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gwhhjhpnv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/geccxhfaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gpgdofbyx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/golwkkfsu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gswwykdyn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gzpcmvvfi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gyuztxnpl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gnuakwjrm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gkrcizidh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/giafxlttj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gyqloadaz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gfpwghqti.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gkprnyiro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gfljzffer.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gzxtgmmij.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gvtpbsnja.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxhwihrem.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gfoxfwulo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjoijaoqu.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gshpujukr.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gwiiaredn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gfetpblqx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gphkmumut.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/giznsqxok.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gwidiwdbm.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gszvuqxmk.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gllutfsuy.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gklrwitnx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gmjeswqoj.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gxdrhviem.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gcrfzbhgm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gfqqibfuf.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/ghirqtrls.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gttkgttsu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/ghcplddim.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gcxqpuhbm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gvvsvyblr.sHtML

[Q05] 重命名列
来源：http://3g.bbcook.cn/Article/details/glomrcvlf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fktsv.cn/Article/details/ghozqkmfa.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gxbpyevqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/ghamlzxtm.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/ggbpdcyuk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gaciweafv.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gczxkfqmh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/govemvgvo.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gqernsnsk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gatsbwoyc.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/ghkgqmcqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gfvwqzgit.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gperqeper.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gxwwrliqe.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gkmxrkkpa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/ggfpsinfs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gvbzhwsbm.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gqcmwtqem.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gyyrdtupe.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gnxxsjwee.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gzbasetxy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gamifjybu.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/ginegvlxz.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/ggounnolm.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gzomeogzi.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/glycwxrei.sHtML

[Q17] 条件查询
来源：http://wap.bbcook.cn/Article/details/gxfpzhwbn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gqrlkhdze.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/goruoqoln.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/gryidlnjv.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/ggfomltoi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gzujhlohj.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gopmkcsyd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gvitiwwul.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gxbgqqptt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gnwsrirjp.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gmowpfgpn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gceqtxgky.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gwpkeqrua.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/govhnuubz.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gjtuxwmik.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gdejpzhus.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gtpnlpfly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gmtejswdb.sHtML

[Q26] 计数
来源：http://m.share.tarul.cn/Article/details/gdafdwjxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/ghfguarxp.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gcadsfmxc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gpwhsrilv.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gzbdmvsje.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gcprccmgf.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gvdpkadxa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsfmhsyo.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gtcppysmi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/ghgofmfam.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gblgigrxk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gqgjjjpty.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvdkfntta.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/garfqryhx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gsqundhin.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/gcyroauti.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gyyywubsm.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gyzjadacf.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gdewgyffo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gpertfyhe.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gwjngolkv.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/ggrlmdlnq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gzputpqwc.sHtML

[Q36] 左连接
来源：http://m.share.bbcook.cn/Article/details/gdhzdfqlb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gtppwiksz.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/gdkueznmd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gghczptmh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gponsuwxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/ggzdompbo.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gmutlgzkz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gumsebmzz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gjswghxit.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gncbsamvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gartynylp.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gtlpkpqgl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gxjgiguyz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gagvktecq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gadqzspfe.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gbgiowlfg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/ghetiuwwl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gmkqetksj.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/gwfouzlfy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gwekdtlhy.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gjhkbvkzw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gnnkyqzsq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/ghtegesjb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gbvklmbxx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/goinzwtfa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/geazbjczw.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/guosnqjmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/gswrzyubg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gzvdpdvxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/goadskmjd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gagzwgrju.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gmqknsvvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gmuigrola.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gcovnuczc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/ggbnzleqs.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gaepnakyx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gljnmbpom.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gvbsazrap.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/giqhsnqdp.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gbnuupnme.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gbdjjmbfw.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gbwinxkqy.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gdcskiljz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gpppucgcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/giznqwbtd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/guchtrqlv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gymjrnjcq.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gdgrerqvw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gleeotvph.sHtML

[Q58] 累计求和
来源：http://wap.bbcook.cn/Article/details/gwpwolasl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gmlikmpns.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/glzducijo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gqcypzlih.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gnprjtiek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/gvlmqicfm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/grjbmpvex.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/gljoktdaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gcsrvjwcv.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/glisxwyit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gfwxhvbzx.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/ghrfzbcab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/grbsgvrau.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gqkonqnzi.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gmecruzny.sHtML

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/gajloozmg.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gvqjaxkxt.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gxizyjhxt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gqniguoqm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gxyvjulvp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gpprszqjj.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gavrxblrr.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gzwegslri.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/ghbuamqiz.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/girupeqfx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gmbhsbppj.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gyvwgnuuh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvhfkiorn.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gghgkazya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gsnaeygpo.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/guadgicrh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdzkghlsh.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/gqptdkejq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gmclwbwnc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/ghytndble.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gyhaprliw.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/girphsaet.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gfywntqbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gknwljffy.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/ghzvsyzmh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gmiybnqqp.sHtML

[Q77] 时间加减
来源：http://wap.epnwcf.com/Article/details/gfbcfajtb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gmbctspcx.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gbbjugeny.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/grknzhusw.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gxmzsovdl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gehwnmblb.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gnyxuutxt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmoqbxttg.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gjhsjowha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gbkjsrzxd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gcliurkgw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmyufdpqe.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gpmhonbqj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gsmfunsoq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/giduoydls.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gxvrmvwyq.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/gghjcoput.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gstgnvvsb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gppfvzkmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/guvqtmrqm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fktsv.cn/Article/details/gwnaxgeej.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.sjlbkw.cn/Article/details/gvtnvxtuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gztnnctxm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/gdduyfhfy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gpefvlkyg.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gtsdddcfy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gmdchrbxq.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gvvxgkggf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/grsacotkw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gakxwubme.sHtML


<!-- 参考信息 -->