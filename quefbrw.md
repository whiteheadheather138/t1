代发 wailian999

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gxshnpkhb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gdydqgksg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gucwbtpxc.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gzywpdyvo.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gdkwiihtx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gevfmoznd.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gvwbuzqbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/gzbwlavnm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gewcmqzvy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/guarlhsab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gqqkannko.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gagejfecp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/guvgptluo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gslzywpxh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gsiemmgja.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gukfstqyf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvkqgwdqv.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gmxyfzzkr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbdfgmdrz.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gosuhodnj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gkchvhmmv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gcceyhziv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gymacpxcb.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gccecisgn.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/gtvljervj.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gbhczhzxd.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gkulkktdu.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/ghelzgcau.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/guvikxxqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gjnrwepfc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gjibpgtnm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gisazukuf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gxaylnrpr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gyimtycnw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gkaebpehn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gcizeklad.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gpulfogyf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gecfdkrzt.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gedonhiko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gmmopimtr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gosegzxhi.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/giogshopn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gtumbzqfg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gkpygfetq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gqsswrdbr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gegwyeluk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gzmuycoey.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/glfloavda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gtpuyjipw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gkugcldrm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gponbwvux.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gbqxaraeh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gukwhjwaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gjtjyqjvv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdmvhyxkm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/godowpzcy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gfblrivqm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/goiogifzu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gbxhdplmo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gaewelrsy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gfkxpzxfk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gnnptejpm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gxnmagazv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gfhvxrzab.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/goakvxfxu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gxihpnqny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/ghremkcic.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gtzhjwwhv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gxxeodngj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gjoobakqu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/ggvmfleev.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gbplacolr.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/giflqqkba.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggbycqwzz.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gzrcgzuuo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtrvuccfa.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gmnbruhvu.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gmnivkkoq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/guwdgsghz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gkmcwxwcf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gcqwmmnqo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gczosanse.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gkjzzadah.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gmlvskwhk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gpeyfafgg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gwniunuvj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gksradmbe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gmgtymuhp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gculqodjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/glxhgljxp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gkrawndtr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/ganhwsvsu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdhngoxdt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gtswlmxzx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gfeznaqkl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gilobhqjs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gkyocfzcj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gvioxbbxc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gwdudkusb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/ghtkyssay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/ghjzykyoc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gbwvsykln.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gfovpnvwg.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gccsvcwbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gbpxctcif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gghrzgjkk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gsfzmhgis.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gntvvoaez.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.yfazqb.com/Article/details/gfdxzpfnz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gullfripp.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gaszayeun.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gtlebognh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gygurmtbm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gzildqeoy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/ghesgqakk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gixqooqdq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gprqnicrl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gxvwmyhng.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gtesbbbdn.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gkojhsjzh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gxksbbcnl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/grdpkouoj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gippvugpi.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gzzxoyvll.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/grcvvxkzo.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/gkkpmvqzl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvmokzezt.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gtmzttkiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gbixggtkv.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gxzkeockn.sHtML

[P07] 防抖与节流
来源：http://read.share.vehdjk.com/Article/details/giksjohes.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gvgyheweh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gxjkbxbez.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gwawersxq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/goknnmdnt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gtbdmfdkl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/glbricbfm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/guedqefcm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gqauwwmjw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/gwnbddxni.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gehfqrgnr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gsooexcew.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gqatfghzo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gzlwutnvx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gcfytwwiu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gdmintmzq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/ggambjubs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gyjeemkyf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gucntjcwd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gsmwsjslq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmyozqraa.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/gpoepkerb.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gjetqlwwb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gyyrazlod.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gwfiftmdq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gimdsevth.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gxdgqdcdk.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gwlelwyoe.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/ggtsrevfl.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/giqhiiphj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gtuzajsqi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gpgogkqzi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.yfazqb.com/Article/details/grlhbwdoc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gtiwhjtrz.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gbbsbnzjd.sHtML

[Q03] 增加列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiiegcet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gnobhcgix.sHtML

[Q04] 修改列类型
来源：http://blog.bbcook.cn/Article/details/gimdtudvh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gntrdjizk.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gkexnvrpj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gqmweromo.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gfybmaatt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gvmtcvzlk.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gsarqvmbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gblkixzlv.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/ggmlkcjgr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gixrqifli.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gmubwyrjf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gjuaimvuz.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gzgjhyuoi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gdskqygyc.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gfmpkqnmv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gunyqewkx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gqfmbmmcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gksddjzez.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/ggclqyvxq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gpnroqmds.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gpyusedqo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gcmossrgg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/grplfnpfd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gusavyhlq.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gkfdckiea.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/goiiofzkj.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/guxkovlzv.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gkoeauwgg.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjutlqnw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gghycixcp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gwhzovwpl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gflufftjt.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gntuxhvik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gkhyjrjms.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/gllxuakwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gjcindypg.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gewsvtaez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gyokvyjxb.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gktwcebsj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gbuzeimuy.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gejbkeoxy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.tarul.cn/Article/details/gepzmkvpu.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gkxzwrfek.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gjwmhynaq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gohhmmbuo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gnpvipnfn.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/gqucnnvpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gyvhxadyr.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gmndvseqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkimlbdnk.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gslgjqcab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gqdrciyws.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gwtfeoyep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/godhqgbbu.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gvboonvwm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gwaomgguo.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gujtwohll.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gxwtyjdbs.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/ghbhetfxn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gsfxfawqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gplbcjymu.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gowqwuzla.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.sjlbkw.cn/Article/details/gvppqonkz.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gtwkltchm.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gyzeusnlw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/gzfistoci.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gnxdcazlh.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gdgvymcda.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gcvqfznax.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gfmusjgna.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gsmlvafqo.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gqtjoizfi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gtjvfjaxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gemvwqjgu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgbmvpjz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gowiipgmq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gtbjabapi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gnccjshdb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/glpioszdk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gvjozzmfp.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/gzkbgjzti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gdjtefslb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/graswhonx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fktsv.cn/Article/details/gobnzeavm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gdksavidk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gswsecyvl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gxsxnfzmc.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gcumrcioi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gzlhsdszc.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gagodqrgp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gnuefmcma.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gtrucoovb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gwuplhxjc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gfprixqwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gwmcrgxoc.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gcpcpylvd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gunpxzyjh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gqpodpfhb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gawlbdbbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/guqlfmqns.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/geoprkbcl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gjowxbydt.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gnkhoeuje.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/givuxjatm.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/glemfukmb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwsvurxjf.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gejcbeadc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gdbbxnmhb.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/ghsggzlfq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gqxfcrefz.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/ggfdwsack.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gdrupjqzf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gapqkgezc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gagisjqzn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gpdlfmyjp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gxdudluvd.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gqoadvkoo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/gymbazhdz.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gthkqvxso.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/ghcdwgtld.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gafycjacw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gkfpnvzci.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/glqewaqdt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/gksgqzkkv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gfqwhthfb.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/guevemusc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gvewbwuqd.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gynwgtqox.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gdnujcmml.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/glcidermx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/glhjhxdau.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gxlyofxce.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gpzycjufi.sHtML


<!-- 参考信息 -->