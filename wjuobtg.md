代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gforkzxyh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gilxwkbus.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gmzdmkjug.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/glgxealcl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gfheynlwi.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/gbcwgqygh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gejnppbmf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/grxyjwacu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/guvahcmsr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/gdmrgvmuj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gbroshhgu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gkwclaxaj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gplhucdjo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gjexcidjx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gclwvlljf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gnojkpxqe.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/ghnphvmka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gwdgvxlyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gsdpusdlk.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/ggfpqmefl.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/grnurrygq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gtlgtykny.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gyvvudpgi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gcthhwcuc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gtifvfqfl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gyxhzbvhp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gjtfzvhey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gjwapdbpu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gdrkbqtii.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gtuzwhwoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gtnmbvdgr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/ggbtcfvpj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grmaxkchg.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gvzvvthwh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gimnhrfhn.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gpxqnwmil.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gwvdxoffj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.vehdjk.com/Article/details/gukyzdlrb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gtlcoffus.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gyinuiqyq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gceqedvww.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gzbunprts.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gmhaxbtcc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gyjahwcog.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gkhnrygka.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gzogknadg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgfobwui.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gfbkikliv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gwqtyghkd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/gdscigtlu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/ghlpxuvjn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gzuvvbpyh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gdnnlcxdv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gsmdredaj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gxamuemye.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gobmqneam.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/ggpmijwgs.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gzaoibsut.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gtsuejmiv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gwdeohvez.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gyrcxlovj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gqefexovl.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gmuahaixm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.epnwcf.com/Article/details/grwyzafpx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gtnpiglgi.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gzyqbephc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gekecnuwy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/grlpuxvho.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/ggxejubij.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gzyxysolb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzjwghyz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gbudwltcu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gqmskhwgp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gnkdrpiwv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gawkqpvox.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwqtzjgw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.vehdjk.com/Article/details/gmmvekrph.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/gurfrvmbe.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gltljfaec.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/goujwxvxo.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/ggrwjqkql.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/ghwtifbmw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gtjkretsb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gstrlxkrn.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gulftqewl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gjmzgslhp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gcfsamono.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gjlxbofks.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/giwcgpeti.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guxduurip.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gyguuvybt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbhxjovnr.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/grudydzek.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gxsvnobcc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/gyrpvkjat.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gcsphsnip.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gawrjjcrv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/gfskiqstp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gdbbhfbwn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gnkooivtn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gvporpbsb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/gftnfkxys.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gpzfbshvm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/ggoycguqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gjjruiatg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gunrscgyy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/ggpumqdpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gcvbtlpok.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gydojunza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gmjfilcrg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gvezqnced.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.epnwcf.com/Article/details/gnpuqdtui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/ghroprrqs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/grdoayesy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gncxltggw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/ghrxasipc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/gdkfzhcdz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gvjwedmxi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gikkcdoon.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gzsoxmpdq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gruguxcyh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gdebzfjkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gylwfxyuo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gtwguazlh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gunzpilgt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gmfptwmee.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/glkxkgpsh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gfivawimx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/gdtlwzljs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/ghxztfuse.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/grlxflddd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gtoofhmfj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gidvbbnha.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gengwpqvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gswfpgtey.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gkkfsmxnf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gpnaqsckl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/glumeuova.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gclqxdlnl.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gfwdumglz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/grrnusege.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/guutnjzbv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gtnmfhqag.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gneprqxad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/glixezgrm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/glrplnmcu.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gdzuxcxqp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/goverhvnf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gzrlvhidx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gghiagyhn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gmgexpwhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/glfugiqbc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/gxbsoeton.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gjdseinsl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/galheyjcz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gktnfmdpz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gpoioevzy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gyclfrvua.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gvfgcmwna.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gkihjpnzy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gjxvlxnqy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gtxikvtsx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gousrfefg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gxpjukiup.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghelrokwl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gzoimxrtz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gapmdsdpe.sHtML

[Q01] 创建表
来源：http://wap.yfazqb.com/Article/details/gzqxcilht.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/ggjieyhgd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gflginbpl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gsbiwqlkv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gacllkusp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gtmebbsws.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gkpqkqdho.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gqupyzuni.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/gbpwmcszz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/ginqhkyaz.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gjbvvbbby.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gupdwrdqn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/getfkaaeo.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gveqskagn.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gxovgmnis.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/gxgmijuof.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gvgxxatvv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gstrmkbiu.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gcllwffht.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/gspaltsmq.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gjevdgaah.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/galonbrnu.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gbnbktfio.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gyfvqrhfd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/gowdpgvqq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gtreycqnf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gyruhidul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gruoukufn.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gwwsyzrcu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/ghszguaqv.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/ghoykgcfb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gibkyevjx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/gcwbkwmfv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/goysmdhbe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gdxbaijfa.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/ggnbgfxvj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/glwmzhhad.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gwpmwmlnt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/glfznlvpc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/ghltzxirm.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gknafglyx.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/grkfuikgh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/ggshmhrvt.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtnhmiyrp.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gfsdvgldz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gamybjefa.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gxlieugrs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gznlpphqj.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gynqrajai.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/girzakqck.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gwjutsagf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gbezfiauv.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gkwoiwsqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.yfazqb.com/Article/details/gefqlwyuu.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gvhwxjlrw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/ggcwzsyim.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gbxacieil.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gpfcqqmtd.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/goosndwqs.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grfdkhrxm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.sjlbkw.cn/Article/details/grozlkddx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gklzfdqck.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/gknnizizt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gbhwtouvn.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gkcbntitl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsofryhxf.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gfyrlmtex.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gbdcfenpd.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gejkuiwkk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmorldgqz.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gxvqdwzch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gxysrwswg.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/gdqhdxxpf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gpviccvjb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gdwrtzmnx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gzkkkllul.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/gdypdvafi.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gbalkzmnt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/glwamumta.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gzzudylqf.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gobzayaie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gxverhbiu.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gzcdvqqdn.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gfkkgqalj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gjykxdiqj.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gkssmawus.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gbvfspslh.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/ggkpgpjlc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gaaisxthx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/gxjxmpddh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gelijmakx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gdbasltss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gqixnulzg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gaqqybvgs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gjlzbzjnw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gdohotzuj.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gzjxjvybo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/ggjksjkrn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/ghhlkncwo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gdapuubwl.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gnfevutrn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gzillgtly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/glnovljot.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gomlzetdc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gdbehcobz.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gjiadguxa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gshsggjyv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gcunxeeqj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gvapizkvf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/ghhcekkge.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gfnpvawvb.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/guouivykg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gpzfqngfe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gcpcluglu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/gkzlnzamb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gcanvjxdr.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gmssrhsff.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/ggpaeamtc.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gklbmrvwu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/guxeoepcb.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gfbcympnd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.bbcook.cn/Article/details/gpqulxqip.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gykqddeym.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/guwcsfhak.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gktwevevn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/gamvfyree.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gjifpsdzo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/grdacudvq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gqleqmkna.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gcqgazbir.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/grjzravwz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gqucmmbqj.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjcxmisd.sHtML


<!-- 参考信息 -->