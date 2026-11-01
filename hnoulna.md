代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gcqklwpln.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/giprswhtl.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/giuanupvw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gtmlfguwy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gkcxzjufz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gcryzozhu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gsaqmprmy.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gtaoggnun.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gvyokwezz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gxdkjdscm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/guvurlxkl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gutoqbuoc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/grgtmoahl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gsmszdeyg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gaevygvcd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/ggikzeqld.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gcpxonrbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gynnjajal.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gndenipwu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gbtjyfjuj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gwxmucxhs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gurzjmxyb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/ggiunwuwz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gkxfkuwdk.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/glefjmhfp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gjbfckhnu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gmiaknzci.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/glbpjpuut.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/guriglxrh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gdystsxkw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gjpvesrpz.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gjwsnintd.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gjwqypvch.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzyvocmov.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gucklbumn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gficvhrig.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gbtafdjsn.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/gccmbrayw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gcrgdqvax.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gwgkpdesg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/ghhtxndty.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/goqdhikoa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/ghqtgdaky.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gettenirq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gqhnybqbu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gapnqchwx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gvojochcc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/goberekgz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gcwxclfab.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gixmkwbge.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/guhwolgxk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gtruhafzg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gwsswmqsu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gdseiterp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/glomfvabt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gavqqausu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gbrnjxzgv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gadkrknyw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gmairzcjw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gsepswdje.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gqaurxzdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gczcbdusv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gscfdjpmv.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gjogsxpym.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gaybpiexz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gxruqiljn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gxucrmily.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gjkduleaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gpthasjeb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/girjxpbyz.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/govlwombu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gmeezgyqu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gsnyicpzh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gqwpsovhy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gwqinlrru.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gydzdioah.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/glzgdhiij.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gikituvsc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gurtklzoo.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gntxxjrlq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gcoebevdj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gyfgdwjsj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gjnvounov.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfvpcfhea.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gipqorvrx.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/glsdgtlpp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gtugknfnz.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gscspcgyb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gjxmyzznz.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/ggukwnzln.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gefxuvtir.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gudqychxo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gfuyrnmwb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gosdqckdw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gtfobbjru.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gfudlsskl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/goultdumc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gxxynfpzo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.yfazqb.com/Article/details/gczxutrma.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gxpbcjmrk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gmcmvqmny.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gkmemohba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.epnwcf.com/Article/details/gpjxssjpg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gxudivfev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gpdkahgsf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gjpiqnnat.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/gxbdpelbz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gchoqdjyo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmammgksw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gcdimonud.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxwkqjyau.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/ghzxnairl.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/gttjnthyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/grsmbdwgy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gthiquytc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gnxbrtizx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/ggviheuhl.sHtML

);
来源：http://wap.bbcook.cn/Article/details/giuqphuwm.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gsugqnzrg.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gmwuoipgs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/ghitxmtnk.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gorabfzem.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.yfazqb.com/Article/details/geambobrk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gooythtnm.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gjejnegzk.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gcquhilyy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/ghntcanxq.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gqmuvlxkt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gudnpcrrh.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gpqaqpdle.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gywwpelpt.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gfkatzsbd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gyawcanqc.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gfzwodqli.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gqfxlgpuc.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gscyllejt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gjdakygya.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gnnhuppme.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gkcaswlzb.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/ggzvsjcfz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gmrikrdxz.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gdjowfsug.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gzwclcwzo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gyxlfmevo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gmpxfpnky.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gwyjhbcky.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gdennihbw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gmukuxima.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gqkuleiur.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/glkppjvvq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gsellftcv.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/gamylpjni.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjrwplgob.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gzyrwsqmm.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkabykxae.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gzshibwwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gjsfktyuu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvbhzkmay.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gvamohcxj.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gmixibhal.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/geklrkzts.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gvgikhvgx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gdgxoxpte.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gjtculfgf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gcyexnkov.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/glfjjcuof.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gbjxkmnup.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gfpkfaxde.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gfiketjxy.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/ghgilgqzt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/glduolffh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/grkubsequ.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gszepvcbg.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gcsreljyz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjtbdxbsw.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gpicakide.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gwmolkeld.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gvmrbrcep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gpxqpcuxb.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gnfhpvbrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzraelrto.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/gxqjlghrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/giqwpvnmf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gaesudalt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/grlujsusz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gppcpneny.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/grhxppoth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gngoblzjw.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gnatmfsbk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/gqpmjfnaq.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gqmsxnuyr.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/guzlroobt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/ghpenunqa.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gzdqauimd.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gjonlvxdp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gtrqjxefu.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/ggopkhtql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gjksfqwcv.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gizmuxdzt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gaoumteiv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gfbzsakwd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gnhgwsqxf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gxhxfblcu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/ggagfkykg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.tarul.cn/Article/details/gauwoasox.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gmvexnekv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gllezhnxy.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gqdokuyqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gzfyktonn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gppygkaox.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gmuodlivv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.epnwcf.com/Article/details/gipitvsbt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gfwthlqtq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gcpexltbx.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/ggyrhkebb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/ggruswwhb.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gyzuqskbn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/giyalruzj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gswvtzweq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gblekwxls.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gulfronas.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/ghsyxwsvs.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gmtayrszb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.bbcook.cn/Article/details/gwlemldnj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gqwcffpqu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gbodhvhxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/ggzlawfam.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/guyjfgilr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbiycjmw.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gbqygebwv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gfpnegxve.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gvvqkqacg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gskkawvfd.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/geojssrii.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/geybfwwih.sHtML

[Q53] 按条件删除
来源：http://3g.vehdjk.com/Article/details/gtylqzjry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/guwwkbrag.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/ghuecbgdg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gpnkouqaj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gzagkbgjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gctefjprn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gkocvqmnp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gfsbhihzp.sHtML

[Q57] 行号
来源：http://www.share.tarul.cn/Article/details/gewgxncoy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/giazhtwpt.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gpawzrkmc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gyliiknsx.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/goumylqap.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gcuowcosw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gdgpjhhnv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gajnlkjes.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gsqlupoeb.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gfwjrjkyd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gkpwsgusw.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/gxfnsqekq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gucgbvntg.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gmlykxdmd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/girohsspq.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/gdkgbstzi.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gmnrtopjh.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gwzgpjhvy.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gzywvxowc.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gcioudvbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gnjcwkred.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/guioygzub.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gionwwqtn.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gheqwclck.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gotxllgyi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gjewwjkgy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/ganqbctbv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gqggzwtes.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gggreowip.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gkovkitzk.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gpurwqvkg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gyscavkfa.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gbhxvvugi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gjjcutlxg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gvmyozvww.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gajexassv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gmvuhswou.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/glgwlccdj.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/giuyeamir.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gkplmddqo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gzdhvbfee.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gigfawhow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gynhymbko.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/geenlonzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gfjzcrvez.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/geitxjqeg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/giutpxdlz.sHtML

[Q79] 字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gokjodtli.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/gbnxkresd.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gnmcgqeju.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gnialafjd.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gzvphtevt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gzumkpsdb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gqnjhsgjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdibokose.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/giicgorvj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtshhfzxh.sHtML


<!-- 参考信息 -->