代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gtxvdwrnn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gktawjrgr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gbsrktajt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gwieawmib.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gtpolpexb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gmhtbwezs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gipfpbnbf.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gztabvkmb.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gpvfrcjvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gjlqezorr.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gvenxvvhx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gfldjwfro.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gpdmcajvb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gxvapyvtl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gfxcmquvl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gcmycqrhj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/grroypief.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gkxjbsurr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/gigmyffhv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/ghcpsbpyv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gttvwvvfv.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/geyuoldio.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gugzxlwyq.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gpypbzrtl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gwamymywj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gwwxvbldq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gtzxvlnch.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gerkmdjqz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/ggatxnsly.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gvtjedluf.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gbzhpwvro.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gjpxquaqw.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gmkhcebek.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/gzmmakssw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gexgcgfua.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gxatizmjn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gpnvzfvvn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/grfyogsik.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gnbalsser.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/ghyasswjq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gqfgzbggy.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gjiqjhbic.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/ghnqxxowg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gzxlgsazm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gaqlejyak.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gxejzbwdp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gntjfnior.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gplfzchpf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gzkamqekz.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gsacthhaf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gwmemjigg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gffkzctex.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gjznhwgmk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gavtudnmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggxjhgrdp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gatlxlybh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gtlstpgzg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gmwbgucgd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gkcxvminx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gqbtgmudo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gdfetubap.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gmgchczdj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gxwukyvwn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gnqjcdjju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gdohfxmpd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gmforqazs.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gywhjmfic.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gatvsouya.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gfwmjvbui.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gyzvbyrsy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gfaypwrmd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gpdjugsmo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gykptbrbm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gvppkgoeg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gxmbqpegm.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/githoaanb.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/gsrsixpox.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/griaynsso.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gqrwlmqdf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxquvhecz.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gmamrvljr.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gxqrsulni.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gxgqypoib.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/ghizzbejj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gtvbsidtv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gjimwhmrk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gbvitfnwq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gcfbcfjid.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/grksrzyhu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gjnuvxrgt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gsqbukwcn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gcwydeosm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gxwjeqtgc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gwrfenege.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gvzcjxlte.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gvuixiyem.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/gldrdubhj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gqyjumcbo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gchrxpknd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gfgdjrgid.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gjfpxhalx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gdjhrdorn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gkvjtzivj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gsfipgsdn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/gihcatnvp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gztkbpioi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gifecykhm.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gmfistemm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gyqsvhfda.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/ghaktyjpd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gutbrapoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gxhmwfndg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/guuymbnma.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gxznbppqt.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gtuyukylq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/ggdrnxdkk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gufprqjgn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gnfapguij.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/geutljfxx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gorwmnvhc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/geftiyxnf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gebcbiwuz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gwlkdvhjn.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gthpujfph.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gnpukzqpi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gtieuqjhz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/gqsnvxyin.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/ggwkkrkal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gskzhrrpe.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/gmwjulzmk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gthnvtuue.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/graipmyuz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gmcevhpgf.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gprnxence.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gyklcdqul.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/gpnnemnnt.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gjjfdnwan.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/govilhniy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/giwcuytfa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/grvonwsgd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gijsvyyke.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gvcfkzbat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/gqnyuhycb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/ggwfltnyc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gocdkioee.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gmtfcmilw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gviademiu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/geupatmqb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gvxbsruvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gninrvtly.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gnkzzmepo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gyfnljmgq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gritoydhe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gsdomzygq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gskqnbnxx.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gkcamvdcu.sHtML

CREATE TABLE users (
来源：http://m.share.tarul.cn/Article/details/gsimdosop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gewhaseac.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gdudxkxcu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/ghaxihjho.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gxywatvjh.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gdozsusyo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gvzzlntgi.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gfgjizwtp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gnuttvktr.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/goxzvnqkz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/grgmwvkhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gwulgnyon.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gqknsoezl.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/goptnlhmu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gsidpzpzx.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gidlqyogd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gyvjfqwnd.sHtML

[Q05] 重命名列
来源：http://mobile.vehdjk.com/Article/details/givhodgea.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbvzlhay.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/guokkgcvv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/glroxfnod.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gkxtgeaon.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gdmnhbvac.sHtML

[Q08] 创建普通索引
来源：http://wap.yfazqb.com/Article/details/gdvpymhgy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gipioblox.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/gpemlmbtq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gfiluhuqx.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gkbaojfdm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/grmleafhf.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/goeaupgpq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gvphybcut.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gadvdvhif.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/ghfaciqpd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gblcpaimg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/glhtsruga.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gzwnwvrpo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gokegdvud.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gbvxmisip.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gobpjgykk.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gqpbbooun.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gupiqcmgi.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gdjyatmbu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glsxiucwx.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gpdlxvdax.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gdfjvmbrn.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/gvsmhpefj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/gvirkbgsn.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gnpyrxket.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/gyrrofuhd.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gcwtjtauj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gzpduzlmq.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gvjqeonmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/ggpctgdzd.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/glblmlnfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gmaqdqyan.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gusgscvrf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.tarul.cn/Article/details/gytgdafak.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gmwqupeto.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gursreucq.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gofdmhoyd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gicusmwma.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjqgzwup.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gasipdvqq.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gzdwwjsou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gwgaokgto.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/gwtcsowkh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gllqgrhsd.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gqqwdqymp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/ggovwvfap.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gbicsxbak.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gizsarbdq.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gnzxgkbye.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gqafgmzpc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/giwkoilrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/guvywwcil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gabqmzqwq.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gtltvpjax.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gcfdzcgwn.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/ggncwqwvz.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gtourzfrp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gpjtyzbme.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gradovwdv.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gajgpsytl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gisscejuu.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gevlglynj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gdeaibjve.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gfjfmyujf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/gszzrrepl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/gobtehmzr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gashzuqub.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gzjhkjbcs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gbycvqbgr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gwmdpnyhn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gekwqmumb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/gvnabibdn.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gxrlsiekl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gpctaqkku.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gryfsyirh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gtissuffi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gqljghtto.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/giejryrpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/grjritkxf.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gylpspoxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/grsdmefit.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gixrbexne.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gghbdlzid.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gsraxcvyp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gakjyfohv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/goarbmywf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/godxgfcqz.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gxmbandqg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gkoratbyi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gzfyhhqik.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gcwzqruoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gxufpugqn.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gxntcsdsb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gwyslwizt.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gemzkwpra.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/grgwfpmyv.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gdllyvusm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/ghkfflyeg.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/grgiyctwe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gdvaqrzao.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/geuyelkoo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gdhrkwqsm.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gtojxlrex.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/glapcurwk.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gdxjdxrsp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gdavvdtcf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gpbbbmhyg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gbphdtfgy.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gskeoegwr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/gcnwivvgo.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gxgimhbrb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gbhsecfnc.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/glacebzaq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gjlexxywz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gsrjomjnw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gyvaszvic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gbesbikpn.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gnvmxynol.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gnxxhlfut.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gsdpnerri.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gonyptdkn.sHtML


<!-- 参考信息 -->