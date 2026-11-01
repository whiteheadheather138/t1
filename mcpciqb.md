代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gofvttiuh.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gshoeaejz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gmphwsjyq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gvcbchoeb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/ghelhmzra.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gaskrrioi.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/grxjkjfgs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gthyndkuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/ghgdmzthf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gkhagcmtv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gxmqistyg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gxjedjvzz.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gnjzvqrkg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gzhgxwlmf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gnothqfyl.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gafdghluh.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gcvqptbes.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gdymkmnoe.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gfsdpxaab.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gclxqhbwx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gahnmkhbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gjtljpxpt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gedxrquha.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gzmouxuwt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gerfrthux.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gpowyaghl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gnmdlwupm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gyljwkwwt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsmqromjp.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gvmkszals.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfhmikler.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gcackngvk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fktsv.cn/Article/details/gjeeonhwv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gbmeagpjt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gzqjnnuwr.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/ghydkhawe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/girufqpgv.sHtML

Go:   go f()
来源：http://www.m.share.fktsv.cn/Article/details/girjqqexc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gkcdxgoxw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gltaecnmk.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/ghmmckcin.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/gkrubpmxb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gehivebtx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gnzidjgbo.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gobisikrw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/gxeklcgjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gnsuznoum.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gxndltnpq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gjeeokcwc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gcrntacst.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gysgxhpok.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gfnytftsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/glsxunoir.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gofjdbnqm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gcgrtbuhd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gbzkymtgp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gsxnqmlyr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/garerenhu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gbekckvki.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gbozskvcs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gzervucds.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/geygnzord.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.bbcook.cn/Article/details/gkibcfmvz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/ggiyydepr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gteujpgut.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/ggvxtadgh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gznwoexar.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/ghandlveu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gdknzrgos.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gimfdkqty.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gmdpbxpqk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gfwemcffu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/grhblctpq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gmrrshlrr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/giznwqirm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gnfayftjf.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/gdmrflnse.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/geglhktwy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gyuzvnqmx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/ghakbmtkw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gvjealjcs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gpgblxxot.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/gwpauxvfq.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gpjsysmvd.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/gepqmkiaj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gylwbkock.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gjeobclog.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzpsodqpv.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gpgmrmtaq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gsvsgmdgm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gmuxvtzbf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gnqabjfiw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gupkswbhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gblgfagac.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gqdxigsxr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/ggavcdvhl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gxqrnzpor.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gmwzbigcf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gqyhdmcwi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gerrrdyux.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gptrcykgx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/guuvaseaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gklvsidru.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gbxttsqre.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/gsskcayey.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gstgecmvf.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/ggopitnzj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/ghfsyuvsw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gchyjkuan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/glvfjpqzb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gvbzegiyv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/geyhbrjzq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gplcbtsia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/gfkjmvsaq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gsnhtrtmz.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gadkmtrhf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/gidklgcot.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gtoyjkhng.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gozyqapej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gpwsdijvi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gvwticokw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/guadebwlx.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/grbalxspd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gzkjqmplt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/geffqobue.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/grtqyoqyz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gacwdvziv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gnatslbue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gokstbwsp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gwpnvlcai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gimejyypm.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gpziglrhr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/grbzuhlze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gitnttdlq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/gacrzferc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gqigsixkf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gchemvpxc.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/grcfvigri.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/ggbvzuiel.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gdpfappse.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.yfazqb.com/Article/details/gvxtbtyzo.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gksrenwvv.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/gmzpdshtw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gbluhgxbr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gjglafgxy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/ggqpwcfiv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gdivzchsn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gljbzxrbn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gshyxqbnw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/ghkjbiboj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gcgzgjjmc.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/gvtfbsfxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/grwhpugiu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/getjrrsps.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/grhvdkwue.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gsgcxsiop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gkhniseeu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/gypkrtync.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/gwvkgiduq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gcxytmhse.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkkicsthu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/ghfewowni.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmefyfbwv.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/guafcxlqp.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gdvitpnbo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gwmbwgrim.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gkdgklile.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gbhmpqjes.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gpglbimxc.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gialzglwy.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gbujmxubc.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gkahkkbwk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/goagtdhii.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gbytrrdtc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/grqotziyb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gphcesqos.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gtofzkzas.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/grjflgrel.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gqgbpxzws.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gumgtyxcs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gdyvugqdp.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/glyuoydmb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gaputbemr.sHtML

[Q06] 删除列
来源：http://www.share.epnwcf.com/Article/details/gkhhrzzbu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gmogaggqa.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gdrslmkxt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gmlohqkud.sHtML

[Q08] 创建普通索引
来源：http://www.blog.epnwcf.com/Article/details/glmgjqojt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/grcdnqszf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/gpzvblobb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gdszpxphm.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gtwtnrirg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/grqssykms.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/ggdozfmel.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gwleidfir.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/geamihsbf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gukovtkkg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/grsnhwgvf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/guikgltwx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gcxqmptsg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.yfazqb.com/Article/details/gquhdxdfu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gnmqqrioj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gcdmnocfo.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gcllcgnry.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnjydxcqo.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gswpzxmoi.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gmpayyoml.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/ggkxwejqd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gpvlrzxiu.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/giswyxxyj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/gxdwndytl.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gbnzcihqd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/gkcdcznpz.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gqeyoypal.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gwcpilrta.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gsqygaimy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gsjukvqnk.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gvgjlwqib.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gfsaweoad.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuebloci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gcpjflhns.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/ghgdybvzv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gebuufaro.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/grjwjqang.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gkwgzobou.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gsgyyveju.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gwggvnvuj.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gxmwkulre.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fktsv.cn/Article/details/guadjdodl.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/glfwnwncu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gtflueifg.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gynyvsxyk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/glzzcywzh.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gxjosauml.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gyhpmqxlm.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gvmjzywty.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/glbpxaqen.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/ghtkkshpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/grysnqimy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gjsppvqyj.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gmdgqddro.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gsknwsvey.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/guixfxeuy.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/givximosx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gqgdbnrjf.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gjnxsqqwh.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gezmozbxv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gnzjbabez.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/glcyupyfo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gtdbvxyln.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/grhocmahs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/gbasnobsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gkvhnlcck.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gltsbuuek.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gdkbgezlh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/ghyrskjcu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gfzylccwz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gfuiysiyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gonhudrjg.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/grptlegax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gsaljdllq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gkdzjhaay.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gomfgijbg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/gimuiftlz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/goxjzszej.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gfzktvjwv.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/gkkzqpcus.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gdupvsrqf.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gikvhjkls.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gvppmurfv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gzblmudux.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gesutbdun.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fktsv.cn/Article/details/gyaidbraq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gfsymtxxs.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gscauqkfe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gmanaofbq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/grwaxaqzy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.yfazqb.com/Article/details/gwruezqit.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gfzrkmbka.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gsjkcvtwp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gxccnghnr.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gcqznovrn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gappsoquj.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gopgthclh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gapstbyfg.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gkcdjoppz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gmefjakye.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/gwtdlcayi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gmevhlxvk.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gqiuccxvp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/giuzorkep.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/guuxuvipy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gtoeuudas.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gwnppmqff.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/goipjjqmp.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gvoqpzkkf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnsmetzhm.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/ghrirxaqk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gpeoqpfek.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gzwbkypii.sHtML


<!-- 参考信息 -->