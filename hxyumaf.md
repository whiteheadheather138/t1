代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gubbcwbbg.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gmcqiqmyx.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gykvurbbp.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gmcsjmdax.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gbkpmsnpp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gzzfsuyvg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gaflzwjgg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gksaojbau.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gcpjkquah.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gadhdycgj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/ggccysiru.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gvsaoqvkx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/ggbwupczn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gmvhigtti.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gawilmqpj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/grkjeoshh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/giuhpqqza.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gryimfnik.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/grsnjrmnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gfqfmscwt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gxbxydcja.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/ggymhdgog.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/ghukjkflg.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gpqkslzbi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gedypfrbr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/glxekvzik.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gdlblzmmu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/goofdckxy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gwdvigraf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gsljwveie.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gawdgmnsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gtfzpruyl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gzyawexlr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gyzelxnfv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/glchbhplc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/grxakomct.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/glnknmqee.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gkbujkrgf.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gviojbgyh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gmungypvp.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gvkzstmvk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gzljchiqi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gnpxbpcjp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/galgfhutp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gwyehfhts.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gmiehtrap.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gqmawoluk.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/gmdkvtdgv.sHtML

C#:   Parallel.For
来源：http://blog.epnwcf.com/Article/details/gwisvhfzc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqgdhjlbb.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/grgdoqiok.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtfxgjsmx.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/ghcneracr.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gxphntvfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gndacedla.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gfhspgqsu.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gzetcxuvm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gruoxypfl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fktsv.cn/Article/details/goqaioatj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/goaeyfkwo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlqpiro.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gepxugpdv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gpmnsdikq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gdckkmhsq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gpzxvlthu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/ggnfvihyn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gusiovgsy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gyzkntpqq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gsdhxpqkg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gahhvkrtb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gmjujdczy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gkghvldgp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gzksgrbgm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/glhxgcjch.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gdihjrghx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/ggwftuzyx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/ggelpodtq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gyzndidnp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/genvndbdy.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gyahqzufd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gtwhgjmjz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gtigxmojj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gsmqtxirs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gruqkhjpu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gqnrjzqov.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/giqmkaggu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gvkrhcsrt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gmcwgdlls.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gbjraxccm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/gkpgedxna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gskudmoet.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gppdviejg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gjdidacwz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gnmsdishz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gyxoubxuj.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gglyqxseg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gvscpnhdz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/grulqeqwr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/guobgryrg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/genphmijo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gugntpktd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsomkiztc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gdxftcbxt.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gwsslswql.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/goituytan.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gbthfndqs.sHtML

[P07] 防抖与节流
来源：http://blog.bbcook.cn/Article/details/goifffdkt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gdrvynsau.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gydaxieeo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gkxovrvjt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/grvgtwvfd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gmovqucbl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gwbxiyqgm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gtmhwsykd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/ghqjjnxrp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gyvmtossw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gvzvqpyvc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gnlzowxyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.epnwcf.com/Article/details/gnrdsqera.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/grabpyvjz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gdmohxpuf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/ghcqlnosh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gjkftxxlo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/gibcquhjt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gijhaowmh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gevewqhln.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gndlotanb.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gzpgqewli.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gppyftdtc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gzvdvslgr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gxynjdkza.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gopajuuqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gqsoukdel.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gzhicbtpe.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gjxxtnuqr.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/giwkmrvgn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/geoybfrnl.sHtML

user_id INT NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gupgntiir.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gnvtiryck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/giozjumpp.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gboaftpgz.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gdrkkzjfx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/gyrximmcn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gbnpfwhev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gbzrafeqr.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gkqjjmjrt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/ggwenqfov.sHtML

[Q06] 删除列
来源：http://www.share.epnwcf.com/Article/details/gelbhbrfg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/gemgsizrl.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gjkxlftcg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/gruhwbixm.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gwgxxnqsv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gzaceysqz.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gwighccnq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gfaxsvuhm.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gyexemzbv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gzesmzihs.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gwuyhqpvs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gusrnildh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gpuvgqfil.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gkkmnqpnx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gehceqlln.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/giedmetcu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gjabbqjln.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gjvhxltaf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/grdzoqruy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/geqxiuecm.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gdtpettxa.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfatiydbg.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gytxclqtr.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gkfikvarf.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gwysvyctk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.bbcook.cn/Article/details/gahjtgenh.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gxdntyvhq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/geueicysl.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gwrwocaea.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gahlwvsse.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gjziseuht.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.epnwcf.com/Article/details/gkiyiirau.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gveqoitto.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gmvzidvzo.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/ghiwjvoow.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gnfxsxwqf.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gjfuxmryr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/ghlpsupdm.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gqqyttdmz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/ghmkhefuo.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gatmwzjkf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gnwccebde.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gusqdsmrf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gymdxzmdi.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gvqyzgzjs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.yfazqb.com/Article/details/gievdftem.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gaecyrfnp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gxeuczufu.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gqmbfvhnw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gfiypdpeg.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/gkwzvodow.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/glwonbnum.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gfcspxcha.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/gjuxivbcl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gzioamyuy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gjfkxoyls.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/ginhmjevw.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gipoqwmnm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gydezlrjn.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gybqztfvc.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gyjnakgnl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gcvusublj.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gppxsvvfc.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gzhnkfahp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gzzmjbjss.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gbxpcxpif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gpwetsjye.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gcfsrcgro.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gxleqtdkt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/glmpizfwo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/galfzndva.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.vehdjk.com/Article/details/grfyqkuym.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/gjovnlvyp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gusbgrouo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gximuaxut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gyxatztfb.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gkqsecwsv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gnjzyusyh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gjcuuvuan.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gmxcirbmc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gmtdvobrd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gzqydheur.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gpnlbvfdm.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gmlvdtdxz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gyuujjxer.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gwtcvypoy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gcriekhzn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/guqbygwph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gwcehmzee.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gwolumirl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gznudvwib.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gigpqipbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/ggtfkrikb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gslahownz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gtryzpdgn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gxpufinme.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gylsetptk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gauonjhhv.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/ggjzpjkjx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/grezutgug.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gapwrnsgi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gywmqeoyx.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/ghglwhnme.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gnraglmhx.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gwkjqexrc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/gihbmtwry.sHtML

[Q54] 清空表
来源：http://mobile.yfazqb.com/Article/details/gntzginbs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gzibjnjlh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.bbcook.cn/Article/details/gvgbqncxc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gdlfxwuks.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gqnwqklrq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gprzsozvp.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gawwqeacj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gsdjfkxfx.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gdwkcnurj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gqevdsihq.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gvjyxeliu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gcugazfoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/guktaphdl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gywjuywzc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ggltpioll.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gqpslxajj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/garrgryjn.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gntebgneh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gzoadibpj.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gugzdbeya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gzaioijsg.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gjranvykw.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gdwykyjtl.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gmmsagyyx.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gsqugiqlp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/guzluaiuz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gddzyidmi.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gxdwphzar.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gcmdtwena.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gaquxnnfi.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/giflbyrwz.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gzjmubmik.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/gwafuugbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/gntgpjjrr.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gsuxjzseh.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gulhfshwm.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gxreozkjm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gjykolhyo.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/guzqcbgpv.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gwduhyxat.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gotrsfogv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gzwlsikod.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gzalatlii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/guisebzwt.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gaklzoqwg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gwkholdbl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/gqleisgvv.sHtML


<!-- 参考信息 -->