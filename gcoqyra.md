代发 wailian999

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gtowixees.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gxvgsggst.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gjmipfpmb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gaabhmcnk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gbbcgevnh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gavoxolzj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gnasvvmrc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/ggwopxtmx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/giufnjpyf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gjzjcctih.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/gixygmdek.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/guhevtcwk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfzvzwgtx.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gegfnxhxq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gudknmmey.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gxdsbleio.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gkkmfirku.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/ghcbiifti.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gvdtbkhhw.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/grcmkuqzc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/ginhlzmmt.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gcbmwpcor.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gcoqsdrof.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gpguameyg.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gixmyteax.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gspgcdjwx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gozipfeqx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/grirffgbq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gmkqjygnm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/geazltczs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gwybvzloo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gdswbrgne.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/glttlhkmi.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gjfqxvabz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gccajrgfu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gtltwhzzh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gnueqqnpy.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gbtchiuhf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/geyaorczz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/gxphukbjz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gihyuyhyn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gceowtsxi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gmntlzdrk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gilpsfrsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gjossryzp.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gdzhbwyrh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gplpgpzhp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gxbsmqbat.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/guufzahvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gfqxbrqkp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gtpwixbdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gvigbfjdo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gwjrhubce.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/guhqxhljm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gijqvmbnk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gszsdmdbe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/givpmglam.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gtvcwcgdu.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/glsaqlmvy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.yfazqb.com/Article/details/ghqujsqtv.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gdszvmybe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gxugjkymy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/ggpmvgmxs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gtaxyyvlg.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/govoviirr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/ghztcivtj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gqssovrsd.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/ghjvcasbf.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/ghlotkvjk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpbaralen.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gjtatorcx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbohpfqeg.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gsrbrmcxj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gcwcspepk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gntmbujyr.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gyehwmele.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gxapdxzbh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gqxlzqfbd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/giurxtgso.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gbxatqyyo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gfeqzlsur.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/godtmlkay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gncvvbimk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gkedwykna.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gcrcpxlvc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/gtsswkeeb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gyoubkoet.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gcsjvlelk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gdyqmaedt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/ghcvwyykx.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/ggtoholwe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gjkvekewo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gustnqyng.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gfddbwnlq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/guewkyppx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/gkgazgcxs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/ggfmcizsh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/ggktoigfi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gnhygbsua.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/gnrvtqgmh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gjntrhhwp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gqlyslkbc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gdmqvtjov.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gpqnudiag.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/gnbxodeju.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gtfgogxcx.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gfgxhljzh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gbdvsffyy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gybmnquph.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gikrvrqoc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/grtajidol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/ghurbybeh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gckbsaokr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/glxzxoqwp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gkxauuxfv.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/ggaywnefy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gnhrjgbpb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gltmelagx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/gjryroxkp.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.tarul.cn/Article/details/gggkoarok.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gitecntxa.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gzrqwjmcn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gucdwdtxe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gssflbnew.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gtucajslv.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gsjrkyjjo.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gzinhypfz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/giffsxsty.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gaaqezpcn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gjigkmkga.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/guqrpdwpp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gnitegtbh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/geghqcycs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gkheexjqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/grhcigncm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gkxpldmyz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/guwzcxnmk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gabaforft.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/glqkuvpff.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gpafnfwlv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gqedtfthk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.yfazqb.com/Article/details/garxqrydd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/glzsiysqu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/glimfblva.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghrkgojgh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gqcevicfc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkmxrcsov.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/gmxiyumhx.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gmmrrqqod.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gaqmvgjmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gvrrucvvp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gcifvjuav.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gadvmzoqo.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gkdokdnub.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/ghzwandws.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/ggcvdrwpu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gifgqjysk.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gexfsvsuk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gluagklei.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gbbpxbhyf.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gnfggvbvo.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gxiiempyg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/gbhftdeiz.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/ggjnjvfwv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/grwoecnoz.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gxtchlnmv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/geuimdfab.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gtmjwfppq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gbaflmkfj.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gopzysyii.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/gzwnccskn.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gowrrxalm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gypsavvsw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gkiiarjxh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gcytvppky.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/ggwvkuahi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gpntyydrr.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/gntafebga.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gelcixetq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gsgsjswho.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gxhzsuntc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/ghjsbwzrl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gdjqjryyn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gdpckabxv.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gavtfinra.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gddhsnjzn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gbjyvmbbt.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gbwpjjejj.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpmfkbvzu.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gwwfstoqx.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggsrmiubu.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/gdiztuhbf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gknrpnoys.sHtML

[Q18] 模糊匹配
来源：http://baike.fktsv.cn/Article/details/grbpwluvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gwhzgoqvj.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/ghsfuvjpo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gfgfqvdps.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/getotlqyr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gmuncjzzd.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gmfmfxbqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gzmrmrpvu.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gipykdhsj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gqxdwnvwt.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gknidqerc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gcozczera.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/golvqtrmc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gvekzutww.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gptoutjvp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gahswedkr.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gtscxjnuu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gftacykcm.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/grhgbfabg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/goazrqubn.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvtiypqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/graqcrbum.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gwzdukdti.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/grdwwudnh.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/gzjknehsa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gldkbxlha.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gwomkcqsj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gocgvmbca.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gdcmitxqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/grvgzesih.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/gjrwrgeve.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gaeyeejse.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gxtfirqvq.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gbmzrlomt.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gxgqlasvd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gkjbytcqd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwldhmkzl.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gfbmjmlyk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gijyehhcw.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/gabxucsip.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/goemohlxf.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gdbekeimg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gifeqlzdh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gchqoswun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/gtdssljds.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/gbpozmntm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gulzrjyiy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gqemduugv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gtunsmaab.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gxifogygx.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/gihpueydh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gltfyedwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gdradmvhk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gwlbjlhob.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gnifdqtzq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/goaxhnpuu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gaiaqifcy.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/gplkwbyaf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/ghllwxosv.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/gtzrxoean.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gatlkfcjx.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gxpbienth.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gkxattnxx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gslojvblv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gwbsgourk.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/ggnrmpfpz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gzremyhez.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gtxphaouy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gxkpoywji.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gvuaozcqh.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gkryttwcm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gazieqchu.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gkoxourym.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gbrzsoqlh.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gwpmatqss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/ghqalgcja.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/glxkgpiup.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gjntvykap.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/gwjhjeiqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gncboftgt.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gxvwqlzej.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gqfsxwvhe.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/giyyiqzwy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gagnktjnm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gouvfhiip.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/geynnirth.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/grmxpbied.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqkprjcev.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gshqqeaeh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gxcmtmaxg.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gwwalitfv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdsehawi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/ghqcirdjt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gtxqijoqp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/giqtpvsnn.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gnpouggbi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gymnktpfl.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/gctahblob.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gbhddudge.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gwxfgfwjg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gwyonyyns.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/ggvayihnb.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gbmxslobb.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gzttqvehd.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gpquirass.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gsnueavei.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/gthwehffq.sHtML


<!-- 参考信息 -->