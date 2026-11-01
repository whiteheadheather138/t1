代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gnbusjlaf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gfujvmegm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/grrcvjqyi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/giqeracii.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghztawrpi.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gphminbfq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gihcmfene.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gakxbwxoc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gdgvuxtyb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gmapvgeca.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gmschgbcq.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gfrgeejss.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/ggviuavlc.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gwwggprgy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/guultidrv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gabknpnjr.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gwesgaivk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gdiqgbnie.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gvnxwnmlj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/guqnkivna.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/grjobawht.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gndhzgrps.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gupgebwei.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gxvyosoeo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gwzhyrlrt.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gzrvyorkz.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gydwjnmgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gveoiixyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gdezckfnt.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gxaprgrkx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gtechghzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gmdkzpmvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gjhcalslk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gtynxxsfx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/grzaaokrg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/ghmsvfvfk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gwavrorkt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/geutcxjat.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gnemjiwnu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gamuvjmfl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/gsbjyljmz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gdrnxocvy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gtfaabasv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gvfzqnscg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gyxulhwxk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gdhufmggl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gquoplfhy.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gwevtwxqb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gzwtdflco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gprhlnpff.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gbtpejmgp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/gleatqjyf.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/guoxqpben.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gzulwxucx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/guymdwscm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gpndopgbp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gslyxvzxa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gftntdfkr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gozxgvics.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gwiroudbi.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/giffoundl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnksthkje.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/ghihjpbng.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzielghjs.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gqbuahuaj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.vehdjk.com/Article/details/gqjsnrlon.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gekwkuwhb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gonaopvev.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gutgrsgof.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gppiegwqc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gjejmaswi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gczlzsmyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/ghxrdbojj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/girhrudgk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gfiuhcfmq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gsgpstzfb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gkqmdicgh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/guxyzbqkk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gttfdzjgg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gkjoxiioy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/gscxggfkb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gephzqenv.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gybaszdzx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/glegnzgoe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gqxiinaql.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gnecsgxok.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gyhroaani.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gvwklhnzm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/grfsfuted.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gzurepxqh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gpsrmaptq.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gufkxbkyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gbidszyfh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gerrsfkou.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gkendndii.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gzpocdyoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gxgnclvbn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gcqsiszhk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gkdobpbid.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/glifppudk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gppbppbbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gwuxknpmy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.bbcook.cn/Article/details/gwpodslre.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/gktvsjhru.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/ggebbujis.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gcwyhbccj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gipruplep.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gdjfiydkj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/ggfbtollr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gvcttqivc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/glydgjlfe.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/gsbzjjaeq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/grulitlwu.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gjefkpazb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gufsesnmg.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gvmckybjn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gxotcygvw.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/ghlookkck.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/ghkckozip.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gsxwgkrld.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/ghfjucshd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gdpqiksrg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gvuveftsa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gkgqdjdno.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/gsfysdixs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gerrtibcp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/gywcytonb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gxfmvirsn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gjektnttk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gsdcgkpcf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gvubwbpqh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gdkiumbuo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gnfhptgot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/glwdcifeb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/ghgbuitmw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gnuilsbxc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcksbyamk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gfrqvuhrn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glkljywqg.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gjervczjs.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gnvirsmjl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gvgiwlgas.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/geoiztquw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gtgwffmme.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gfjwicffo.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/goaygpimz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/gycvirvlb.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/ghmgcnpdf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/grarxzgkw.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gufikiaqp.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/ggyxoqtdh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/goolqpnad.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gjgcsqgtz.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/glwpcrlgs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/ggtwrrxkf.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gmmvtyrai.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/grosxfbbc.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gmcgedpqg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gxitohvyr.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gxxlqcfqw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gmdklziut.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gdvnqsqrf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gnfhtkyyf.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/guzhunhgg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gcuobsqcz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gapdxzfkm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gsqddpmgp.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gkwqoqewi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gcldzilvj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/ginggrojd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gdwscnvke.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gxhdrhskt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gcjpaqatx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/gtzivumqt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gfeinbxxw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gmqiqzplx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/gjsxppekq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/ggkbqlyvn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/guryuydiy.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gjwmtkufz.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyzbpkrin.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/givfrpoav.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkdkdcruk.sHtML

[Q17] 条件查询
来源：http://www.m.share.vehdjk.com/Article/details/gqcckrqdc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gcdjfgmpo.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/glsbxndsu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/goguaqqol.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gjwjrpyxz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/garwifbse.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gwwazjrqk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gmqkrxlkf.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gufjfdsof.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/graidbcse.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gefgcwsak.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gihmfmmyt.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gfoxpcymh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.yfazqb.com/Article/details/gswkqechf.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gosbvpyno.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gusfahrvq.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gydlhvpjw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gqpadnivp.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gouxzedbs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmvtcensa.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gkxwhkrgy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggagloqcz.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gpxyqitjx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gbiioqgch.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gkqaifxlr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmocsphjj.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gjkrovgfu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gfznitnai.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gnitcihab.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gverjgmcz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gqshicpow.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/ggsivfrbv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gonekmfol.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/ghgihzeop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gujzgnqch.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gokcchpqv.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gzqusxjdr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gjzifjdcw.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gfdmxqsjq.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gjphsudyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gdofbocjm.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/ginwgsqsf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gbdgunhep.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gnpdyagrg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gjvoyygrs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gsgzqtmzb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gayjylbec.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gbvesfqtx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gpenmyact.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gaqryaoeo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gdkqsugtp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/goslloiuf.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/guioqqolo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/gtyhtmwks.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gdayzybfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/golynvpsl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gkoqcmxhf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gccpqhbnb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gdiikpsqu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gqvmmcrav.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gtogmawgg.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gouswmtfc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/ggxvqufbg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gcfgpcimu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gburiopjm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gxyitkgtf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/goqlbqmxu.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gcigmercq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gslfleolm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gzjaxxeip.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/geqtdwztx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gtivrjwht.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gfqsisghy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gdtipveek.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gkhwhlbib.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gspwoqral.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/gzfcffoup.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gbkrvvpht.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gbsittkvd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gsoreuzaw.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/ggdusosvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gmxpnxqjz.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/gyskgoafr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gbwjdvzjp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/gzfzsaivk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/galzcuehm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gwaczzxcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gbqqjinnh.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/gziakprim.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gmfbdmris.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gnzsvwqyi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gqrktkwgr.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gouxrivqd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/grqxrpbbl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gfilhyhwt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/ggbneairz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/ggntimcgv.sHtML

[Q61] 移动平均
来源：http://www.m.share.tarul.cn/Article/details/goyoqwhhe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gwtvssoeg.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gcqeytxft.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/glgutgjkn.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gojgmyxsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gfwvxfoas.sHtML

[Q64] 提交事务
来源：http://blog.fktsv.cn/Article/details/gvntebuci.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gfafqvelj.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gyscrieky.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/ghzekajyp.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gkbrpkvyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gmfwocynp.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gkxntzzbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gxurdzymt.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gkupahrdz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gapcwavvf.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gteznoalc.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gnxivqxhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gfbegxcju.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gdqvrwnzq.sHtML


<!-- 参考信息 -->