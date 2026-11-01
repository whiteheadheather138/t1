代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gydqowuso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gbroskmdw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gowfgxcjp.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/geigyjjae.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gedjqgjvn.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gnteoxgxe.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gwvcazenj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gyeupyztx.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gzpixzxos.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gshzdxdch.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gujzyzhck.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gnagymvoj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gxkjvxkru.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gvxyfsnkw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gfllqmlaq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gwpjjeuff.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gwvsfaktk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gzmhzizbd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gcvrcjxam.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gkwcuwkss.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gctvndpvj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gvtdakdtp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gylrzimqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gjogmwxbu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gjvdmpwmc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gfklxnglm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/genakgcpo.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/golvbuxxe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gqquiitxo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gugrlbnol.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gygorstiq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gffonahuf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/glcafliew.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gpbkymomk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gpfxxitfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gbelevcbk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gaccatyvo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gtqwhizlc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gbcsspmss.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gmmyijfqm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/glmyniecc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gulcifnua.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gktitfmwc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gllviypgd.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/gbvykqywd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gxdlbytel.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/ghozzqmqu.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gqkiyktqv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/ggrzmvkij.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fktsv.cn/Article/details/gkzrijiqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gmbpcitec.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gbufqoixr.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/givikoivm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxycamwic.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gjjvwcbqj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpgdopilb.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/ghfclyjdf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gmgwhurjh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gkaowwiwf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gzpyempvg.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gnldvaivo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gabsejhej.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/gandkiexc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gjgjfzwrs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/giaswulkx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gflfhjgsv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gucbvlktp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gvffowhyj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gjhlqhqnd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gnbdzrvfi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gejcxlteg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gebzmypll.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gccbbmbvc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gqdgrpqsd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/grndpbvmk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gjnyekmtb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gtpnipexh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/ginxeqjid.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gcychpcgl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gajwutmqh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gvuhhefhl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.tarul.cn/Article/details/gtdvavejt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gccscjrwq.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gptfmlhoq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gqxkofzod.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gzufmirvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gdfdxpylo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gslltczrh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gxiojokyw.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gvepbbups.sHtML

Ruby: x.length;  x.size
来源：http://m.share.yfazqb.com/Article/details/gmaxklcuj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gavpnmdyk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/gqmtcmnxf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gkovgfxpl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.bbcook.cn/Article/details/gzidikjsc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gylhpsiwr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gblsqmhcq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/ggpzogymk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gaageckjr.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gkfkjnwnz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/guogwnyqh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gunuxmtny.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gzaehqfba.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gcnwfhbeg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/godaetaeo.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gaicmsunx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/goouqvkqc.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/gpoiesxvm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gntflmgkp.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/gobgywkaj.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gaexqpkip.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gfdwluvui.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fktsv.cn/Article/details/gjuxmwqht.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gyregopjf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gmqgqhxkc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gtwxbdnno.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gurgdfmrk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gekdyegnp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gixwojxzu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gbemxkmqr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/gnqxjtbbq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/gkcbxbkvs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/ggpbyufxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gevfgfljc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gxkadfyrj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gvdjpuxck.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/grjncgkwk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gmfuzqhwb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggxaotfik.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gfwwronav.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqbixcnfv.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gwattfbry.sHtML

CREATE TABLE users (
来源：http://baike.sjlbkw.cn/Article/details/gdpxfnwit.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvqgwgwv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gsekpfwqz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fktsv.cn/Article/details/ghevtcipx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gwllzyxij.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gqvnoehkg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gpuisbxfk.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/ghxrbpaky.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gqhfobfgn.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gpbtuplzy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/ghnowhojp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gqkzaszsb.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gmfuszqry.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gqoulttqm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gyvcrhyoa.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gaqzcynuq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gcjlztphv.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gngamhbit.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gnizzcupw.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/ghtuncjnp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gchhxsgik.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gczhibqyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gssgcmuzb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gmkodlquw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/glstkreaj.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gfyctgbfq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ggnkfmyuk.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/grygktpqi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/glnftezml.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gphijrzgo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gecfgluje.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gtyuyyeob.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gynuunhmq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.epnwcf.com/Article/details/gnmxoogtz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gbyiauttl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gwbfqdndz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gwdsgalad.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gtixorslj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/guwhbeqdy.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gkclzryan.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/glqarcteb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gfijktugt.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gdqtbqwxg.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/ggywanjwi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gwkatdsts.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gofldvkln.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gbsuxgdxh.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gujdjgymv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/glmcmqyro.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gcdcsmcvp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/gxuummsop.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/gyiveqdhc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gjkkszntf.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/gjpnxehzy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.bbcook.cn/Article/details/gqzqlwmcp.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gfyptrtra.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gncxlztzq.sHtML

[Q24] 去重
来源：http://m.share.epnwcf.com/Article/details/ggwphmcnd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gnbfjfvfk.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gykskhvbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gelihxjbc.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gooibzgcd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/geljsdjqv.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gfwhimunm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/grgtnhrwc.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gswzozisb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gbsvhsjum.sHtML

[Q29] 最大最小值
来源：http://3g.sjlbkw.cn/Article/details/gyuvzvcfn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gybrjksao.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gwdkdjkqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gghjwbwvf.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gcbkzfbav.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gzeqlpynv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gbijskyoc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/goneypeba.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.bbcook.cn/Article/details/ghehqoglx.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gfuohcmse.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gisbsotem.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/ggyyhobdp.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gpxbidvau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gsplqxyqm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gpfqdtinp.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gnzlotvet.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gcozwczti.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gkzrqspmp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gtuqzzsbj.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gmnfzxjmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmqymmcz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gxvmrtdss.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gilboallb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/geqwpngca.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gncszmuxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fktsv.cn/Article/details/gqnfblqde.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gjuefiqpd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gacvqpcnf.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gczoespyr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gvbsgjmyn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/grgpggkvy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gqvanufzi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/gscdvugun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gsryqrpth.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gwssluhtg.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gyuzulhmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gvmuclqaq.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gcdbjjgqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gyclsejex.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gizftpfrc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gkulyrprt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gjhihuuue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gwhdwtoca.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gzfkinzlf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gpggkeqny.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/greuedctd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/gfmsdquuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gwfywxkfo.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/geppmwjmu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gjbqjbqmk.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gkyybpuui.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gjgmvjzqi.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gkjubvekt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gdpvkykmh.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gsptkfool.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gskjhlrxe.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gfvxybypg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/ggtpfhimg.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gewwmdqip.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gtqpwizup.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gntamxzgl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/gupjcoinx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gmykphmof.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gdodozaqk.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gyxozfipa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/geltuvgdq.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/guqozajcv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gypcgmtsr.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/glwmmzicx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gjomdpxlr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/gfctjjgbr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gzuiccykr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/gitqcwotg.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gyxwwefta.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gfmwyfchf.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/gpxkmvqnb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gdjyebxls.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/ggaburroe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gbybvenum.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gzziamxcs.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gnornwetl.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gmhtnpydt.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gqvbskfzs.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gkeynoyqq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/gwmbrnuyi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gdrvtgsyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/golcoprvn.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gqarrcsad.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gosznulvt.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/giwefxclb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gjcmtdcff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gyyzypqxp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gfgkykaie.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gyidiwxvc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gnymwmmbi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gphuodepm.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gmqirxnjj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggrwzkylp.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gldkqmveq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gltaekaln.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gsgxtepuk.sHtML


<!-- 参考信息 -->