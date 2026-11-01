代发 wailian999

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gmdttowkz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gctwhvaaq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gydgrwqde.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gzhmacilv.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gleswuhzi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gszvcvrqy.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gadwwhjoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gxrdiyadm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/ggaeonuff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gcmpauukf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gruzloyhk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gdxotaiiz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gmufasspx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/grxfcouyx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/ghbphtrxv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gtwxxatqs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsehkkpiv.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gywwysjmh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmbitctq.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gsrquojhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gjqyoclnn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gmpodxcee.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gpibatzll.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gccnlntgs.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gsgtwulad.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gnmyfslwj.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gksljcwpp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gkmbxiznq.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/ghzlywhjl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gyqzefmzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gegjnrecw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gdcbnueqj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gfxlphbkj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/ghbyzuhry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gfgckkpsl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/gidkxupcl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gepodutzg.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gipppbcar.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gbxfyllob.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gmtqeuhry.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gvkpjakjq.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gyarvvrlx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gugivlegf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gipghjlli.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gmjqgohxr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gjaeezztd.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gbjxxvxji.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gmyddtsrl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gyoptgjak.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gfxwnthys.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/glivdeumm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gxabnnbyy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gmfablasm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gqyuwmdza.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gslxfftnz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gcihphgqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gmzhdvivy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gceowzthp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gdupezokt.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gkfomvsws.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gtcdbpnjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gffigahpf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gqhtmdcux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gkkeefrsf.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/glxduczsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gccnuvgsc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/glwurqzky.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gvrhppaet.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/graevdiev.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gcumzvbjt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gufwodntb.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gaakcamfx.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/ggbdworex.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbgfvalbo.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/gwbjbugyr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gucguwjyo.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gmuatgebu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gkglsvcqn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gnexxauxv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gimfidmye.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/goduqeily.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gkftwojtb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gxrhwgdmo.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gzvgbttev.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gckgjfpys.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gdlvgmhoe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gwfmkwriu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gocsjrbaz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gbblnkhfp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/godfroeew.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gsnghwmag.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/ggigogzit.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gpvmznwmh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gutskswmz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gvmijkthc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gbdohouzx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gumgevkax.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gxputkebk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gjmmeuvnc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gvevciscg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gyegxezho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/guorfnnye.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gcnwcdpue.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gsadybmcg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gebhmcsoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gsuyeadtu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gyjvukuxm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gfyuliggz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gmqpfcczm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gslmafkvr.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gzxbbjpkh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gzgsaroxm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gdkotjbsr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gurdbdqwj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gvkioyanx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpetttfr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gmfdipgxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/ghcrrmhel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gzshhyeyj.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gsekdnhhf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gckkorjuw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gydmjeyfp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.tarul.cn/Article/details/gjjvslxbd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/gskfrvihd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gvtzyhogk.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggcvujxeo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gwkzmuyfy.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gdqtsfkek.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/givgjoxkx.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gevnphkod.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gwfcndcuo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/gdtwteupv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.tarul.cn/Article/details/gkswvhvtk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/glbzjiwja.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gfldlwzza.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gxfbzjpzy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/glvuwkpzh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gqpvjexbp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/geomhtboa.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/ghskpijpi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gmagmwwlk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/goagvqoyi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/gymojjhqp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gkvwlmynk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/ghbpjpitp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/geakbdalj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjaapmfu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gsbbauapx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gblgoyyya.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gsxpqtnpz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grvifmgui.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gdehmprbs.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gmhdccxdd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gkixjvxud.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gubmqrbgk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fktsv.cn/Article/details/gmkzejcgu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gxkpyblty.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcrwovcc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/goaxakexc.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gmtlenzwo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/grxqntyrj.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/goibbalyu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gxfcoauns.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/ggfstjirk.sHtML

);
来源：http://baike.tarul.cn/Article/details/gqowclzla.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/guxagrxdd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gghuvtlvf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gvndhyqce.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gtxdgykir.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gzyrammjm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gtrimovct.sHtML

[Q06] 删除列
来源：http://www.blog.bbcook.cn/Article/details/geiuubozt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gvpkcrhjp.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gopngmhim.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/gwgxpxhre.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/gobzlqmdh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/giqndqirk.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/guyofnojz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gtpeylyaw.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gkgiruxyp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gcfwinuaz.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gpvvwcvwx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/gxxawywyf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gadcqwnha.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/giproapin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gcyoraezk.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gwmfwerwn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/grmsfytmn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gforvftmk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gskbzcsmd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gmmzilinl.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/glwiegkyt.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gwrdegmnd.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/ggpeixady.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/ghdixliay.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/gkoxvczwt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gpwedtyda.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gjeqcfpeg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gbvmiznwc.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/gouhffbgt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gdidgeijf.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gttnswfys.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gcpbqjunl.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gmzlrrpgc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/ghiojwamf.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gidpybdys.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.sjlbkw.cn/Article/details/gfrnuwuxo.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gmgwgsodh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/ghqoqkoho.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/ggohmisaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gmwnarrex.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gzacspgnm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gncooprzl.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/goybgrmfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvfcsrujm.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gyiuberbd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fktsv.cn/Article/details/gqornqhdw.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gipfsqvdo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gvdlnkhgz.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gwnhnrhel.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gwgnzhsfo.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gzptwtrse.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gfmvoqvtc.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gwwbesozm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gspyailmr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/guyszxovm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gtyirzdpb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gqhyidsiu.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gkifyqfyi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gbhgrgleq.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gbooooixl.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/ggdindyrb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gzcnrxlwd.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/ggqwqeyzh.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/ggdtqwwye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gsyfcztxt.sHtML

[Q36] 左连接
来源：http://m.share.vehdjk.com/Article/details/gddevuclj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gujoggskb.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/guzmimpfm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gsmufpgrr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gyxiiluyh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gpzcvqbsi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gartplzsj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gecmpzizj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/gfizavqry.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fktsv.cn/Article/details/gvevmyrgo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gfwqjfmfx.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gkbrnhfno.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/goadfchei.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gvuxsfdve.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gxwhvjuay.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gafbhtrht.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.bbcook.cn/Article/details/gdpdlqzes.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gnlzmuras.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gxdpbswps.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gvyetmhbl.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gewqlztlw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gvgdmwaux.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gqcmjpccd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gzrezhivb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gtmvzsjlj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gpbzjfnkr.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gdljmkkvv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gloxkslah.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gfdlsrxbb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gtqjcayjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gutnjkljp.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gtpighujf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gypalszjd.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/gzeffjvqi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gtbzrmakn.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/ghwdbwdhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gbpptgpbl.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/glepjpfmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gauaapcag.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gdhhdebhn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gwkzwrgxl.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gpemxkqav.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/goaqixech.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gfqxksljo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gflvxlqim.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gwaqjjkuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gjakxrjaq.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gjwqibhsd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gfyijyqab.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/grtwuvyrs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gupucglid.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gcjuoqcpz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gvejfuhzl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gefbwxwjn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gxvfmhxgg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gdbocfdil.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gmhfjyjqx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/geeaxikob.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gpuejidta.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/grdgxpwha.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gpbfvwkfo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gbfuniofr.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gcwvpycfo.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gmmfafoma.sHtML


<!-- 参考信息 -->