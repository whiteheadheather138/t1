代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gpnwhbidq.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gxfgeuuam.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gwiccpzsc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gdfvrkoes.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gkqzpdlbx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gmcpppoml.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/gtsgawrzt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gzdhwuwez.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gwlvsyowt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/guzdsbonj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/guuxggxkd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/ggvbsyqre.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvyfkrkc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gcsiaxazd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gwukzshpn.sHtML

Java: // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gcxxinxxn.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gxduieqpo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gjrumiedc.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gxrgvpwrl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gwfiyqclj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gntljskcl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/gqfkbdwtf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gjfgkvpoi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gvccrspgc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gjxbqogwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gkzjghcwc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/geqxzdkok.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gywtwfwch.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvdeesttw.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gqlhbcrck.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gewazwnzm.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/glriwrudz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gjiahimyn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gybsvmzdf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/ggbagejeo.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gyspxgljx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/geveqtqkd.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gmpjkisjl.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gubibrbil.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gfacjkqmu.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gwckrpxmb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gpofeowqp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gcqkzrjbn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gezjtstfa.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gmtfhbqku.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gejmkairb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gdtowzqtb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gxqngbeic.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gfsvgelok.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.bbcook.cn/Article/details/grzddorej.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gtyhsmycr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gxnfqyjgy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gnszxmets.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gejmpbjoi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/glgbxtudb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/grluuscgq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/ghixjuspi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gbnwgmmfm.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gonguyfce.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gfwuswwql.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gjbzwjeyt.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/ggfufftbs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gbtahuboq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gfssqbepv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gogsnapvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gxoyhhbni.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gvisokvom.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gxoynjlvq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gtkniqnkd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gmvaxtjui.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/guieixsko.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/girjnbacv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gobmurxad.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gtqgitsnx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gwbllvqpc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/giqzkticq.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gqjdheeez.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gazitumya.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gyesygkij.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gbcsarcmm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gsntnfvri.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gqwqijfcd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/gzzsssipg.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gbhoeeiws.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/glryepizo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geingwwcf.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/ghcrjdizd.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbrmvesed.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/ggglfmibm.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gqhctbgsf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gjsdfrmue.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/ggclfuaex.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gusudvssz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/glsjsuwpr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.bbcook.cn/Article/details/gsfpylwnw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gqcklftnj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gsbcrmbfs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gkwgaxvgd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gqrptpffp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/giavdkqgm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gexyhtpbz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gcccsdmif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/grstsjmzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gekjdyvdv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gahlwtqtp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gdhrauavq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gxveontbs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fktsv.cn/Article/details/gqoppjuuu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gjbnmcdvy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gifjpyvie.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gkqkdeiha.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/grduxmxbi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gcucrfflw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/garsdzzjb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gmugcpypm.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbyqawbq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/ghmxxecuk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gsivqgjro.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/giaoyawmi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gaouynxrd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/ggdlcynkj.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gbgduhdgd.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gkchulide.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gsbluhtpf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.vehdjk.com/Article/details/gwsymjogk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gxpdxwwqp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gbeqzgnta.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gnckwomkb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gyqwxuemc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/gpmkfoahc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gepcczvjh.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gqyqhbjkt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gwzmlklqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gygwyyotr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/grinhpnaj.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/ggscuhcqp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gdkjydpha.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gdyjbdjjf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gihithbpz.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gektkdgwm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/gbnzghvsi.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/ggdjrvtda.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gkwprbpjk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gvihyvdwi.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gnmlddggn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gsocmgaze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gqdwzelif.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/giggtfqkk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/glsvililp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/ghhnggroh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.bbcook.cn/Article/details/gasfhwroo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gywtelisu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gxxbxnlrc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/gklanpodb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gbwrzcvdr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/ggnqhuxkw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/grazxnrbd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/glutbqumv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/geriefkpe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gqxxxmjhz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjiyfrrea.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gfaqukvam.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glqwyuvai.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/grejfmjkq.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gkapbxrkh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gfmjsszqo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gofcnmvqe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/glanelgbx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/grrfykpie.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gdgxqekzr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgqwmqiu.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gcwimcehw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/getfttjvc.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/ggpchrttu.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gerhurhqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gzhdrgamt.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gsllarfme.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gfoeegmmx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gwrqmcmiv.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gyhlzjnza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gnjepehxi.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/ghbqxyzeb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gunyhbmuw.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gzqimvxut.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gqprjpolm.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/gpsrsnejp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gsgdaodfy.sHtML

[Q08] 创建普通索引
来源：http://wap.yfazqb.com/Article/details/gcuepsjns.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/goewjekmh.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/grwoqvcnm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gufwdabji.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gaxatxstx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/giqzhiqiw.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gkatdqebl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/ggluknffj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gkrqxkqcm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gtnaqicas.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/ggoqwpykf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gdhzblprj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gwzphwios.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gtufrsuyd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/gtzpqytpn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gmsqojazz.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gnwonwdyx.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpiwkyzis.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gkcawuxps.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/guzpzghla.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gzuzvgoyg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/godbqydqm.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gmyjhwajm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gxzfvhwgw.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/geubifaeu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gvycgpybs.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gesnovvyc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gerhvxatv.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gkzxfptnx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/ggmejnslc.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gdmqjfmho.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gktdowmit.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gwimkeudd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gnrlcjciw.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gpheuxnqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/ghvzzkagt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gaidghagy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/glfosyibl.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gqrnqdagm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gabzqfvvc.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gfrmgbelz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gzodiriah.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/gaezsljsm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gdhfxired.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/ghytfgvef.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/ghxihytiu.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/giisemgxt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/ghxdkoqer.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gvzxlwmfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gbokzijos.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gpnbyikcl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gzrrwfbfc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gywkjebjo.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gnvoglsev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/giuxdqqtk.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gvlqlplww.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gdedvclif.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gdiqpopmz.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gwqbbayen.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gmndljhde.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/goclgfpmn.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/giydlyivp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/guxvqmqya.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gcxijrvsz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/grpddnfju.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gigvihzhn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcddtgwae.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gemjzjzsr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gzowetyrf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gwdbmzqob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gmsvsrjap.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gaaynumvm.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/gucznwtfa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gwjizfnjs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gohihsvnf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gglrueluz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/giqifgwuv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/ggnaropvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gkxpaltgl.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gkyfuujec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gtdmcgfse.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gdkfnzvmb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gefjaccef.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gkxzcwnrg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gnqbknsvh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/geqfwhvkm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gwzcblnel.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gdkbjphey.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/glagnerrw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/ggvwkdmfo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjcftqpb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/grdeuhmca.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/glfzzcnyw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gvijebwha.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gnwzcofdk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gcegookpg.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/ggdckjsys.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/grmcbhtoh.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/glyyvyiiu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gotokgkxx.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/ggkoupopl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/giusungvi.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gdufnekcs.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/ghrnznacu.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/gcxtdlfct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/ggibfeyog.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gphutbvds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gmtlbuzcr.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gmhjtkeqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfzdcdmpe.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gorindiqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gpywegpkg.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gmuxiqzad.sHtML


<!-- 参考信息 -->