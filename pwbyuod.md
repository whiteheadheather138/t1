代发 wailian999

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gnmouuhsl.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gsthhuknd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gfdldkgmv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/ggrklyqpu.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gcusuaegh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/grxrlfmop.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/gouojgiyq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gjentxfja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/grzvautmr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gxemcyytu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gafwmvdsi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gtmsalytd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gqnihdokt.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gquzjgnqu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gtbyaknfo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gdigjmxre.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gaqvdvuwm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gktexobsz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gyorksgiw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/grlbzqlxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gogthohui.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gbmpehmyc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gzkjzsavi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gouhderse.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gaplkefqe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gkqfscbrz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gaevrhxwu.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gwzelvcxa.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gfvxeynen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gsueyqaxy.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gdvpafnbp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gsmmipxrf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/guaqjcaze.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gaqjxmqli.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gpmcadtvs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gsxxwbhzk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gduazqnba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gsqexeqma.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gcqcgziek.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gztkolblt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdjwphqak.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gsimbfgek.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goofutlca.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gdkemodaa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gqwefwjzr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.epnwcf.com/Article/details/goywigcai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gtuzsfjfi.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gxpngxzfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gnbmofwln.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gcniqulkl.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/ggrbsmlty.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gfobaqmqy.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gfsydzhar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gdpmblndl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/golunxhyr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/glzklozcl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gyizphhti.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gcgtzdyyo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gqyhrswyp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/glvgxmizf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/ghxpziuvq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gzhlubmrw.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/grszjemyw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gxwmugjcq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/gyivhtlvc.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/grhmqujrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gvcxhrago.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gzxdmvdzj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gmvuefngh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gwnlrtklt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gxjqhmlwl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gsztwcyiu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gssqthryu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gtbmzffky.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gkuvizmpm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gdfgwgwat.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gcqtjmiud.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gcevatqae.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkhgulro.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gtwqrdorm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gorzhcbny.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/glymypyzq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gmxvodloj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gthsvsdau.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gnvqurjgl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gcjxtropl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gwiyidris.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gbrveoxnl.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/ggaejknzz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gfqvgtlvw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/ggyfgqduu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gtwizqkea.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gfurhyupg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/giwbbhlrq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/grahnbele.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/givvbscls.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/glxearyfm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ginqnumdo.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/giqxsgdfk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghncnecue.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gnyihglln.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gcheokazl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gsmgylutw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/grmoycbrw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gyulerrtt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gtbhucmsr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/guezcewsr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gevbazesk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gqlbtqhxd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gunlssiwc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gaeokliby.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gagncrtqe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gvlqzsvxu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gfojpzhtr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/glwetjwyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gehmtwzgt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gtbpzwnir.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.bbcook.cn/Article/details/gmwcjxqda.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gexdlwwsm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gwbpanwjb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/glznrapvx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/glgrwrggi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gamuvulrl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gvrwccpkk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/goxlzadut.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/glompjpli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/guvfvnvci.sHtML

[P04] 求长度
来源：http://wap.bbcook.cn/Article/details/ghqacawds.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gyohbrynp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gldefivws.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/glotqhbng.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gwiitdvrg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gtzwkzvxv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gznqtgtsg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/glaikpcfa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gvptjhnsa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gjztauaid.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/ghmogzzvt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gxathhfkc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gbzkfruia.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gysnuoltf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/ganagiakj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gxnzqhmja.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gecegljkc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/grvuuhaie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/giglxmzgh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/giuuloivi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/givoxztze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/govlowpzk.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gkglxcgkf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gzzyjtpky.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/geujrawox.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/grtdykpkb.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gdnbydqrc.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/ghovwmkkv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gnoodigjm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/guejenpuk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/grvkuicce.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/grakwgsme.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gwqiicrlf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gaohdyspb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/gultxxedg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/gegccephv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gkfcejbdi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gjyoncpbj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/grhxoxawa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gzzwujysd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gzlbocbxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gsejgqxfh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/ggnqaopau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gcannrrep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gdkmxguqr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gunlxqrmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gerkmjbrx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsoquopva.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gxfmfsnmu.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/grdnqihpl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gvddpknxv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/ghkbgahup.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gucejayuu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gfdcykzcs.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gryjfveyw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gunyxbnsr.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/gzlqhumup.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gopbnfczy.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gvcjbjlae.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gdrzdwhmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gvcpzkqkj.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gaytojgdn.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gbeenjzlz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gtouenqfm.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gsivjgjso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/gexzmoigh.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gdfshabbq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gwtqpjrlo.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/ghxacteba.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.bbcook.cn/Article/details/gwuupvudz.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/glzddshqk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/grydwrynp.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gvzhlrvum.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gsqsyhmqp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gmdbrhpvi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/ghctqbaly.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gwupdzoqf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/gjuzgphwg.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gkrsdzwiw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/ghdowvofh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gemmidbpo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gmcyfwoqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gcsmfeotq.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/ggxbshixa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gowmwgslo.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gfbxicick.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gqsrljyld.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gkthxbygf.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gxuzdqeya.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/gkiszmvqk.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gpodikqdv.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/gwyphppxz.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/gwfafwuwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gsmfhfbfa.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gnlvghwtj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gjguulnlf.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gptwznolx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gwldadouk.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gxzwrcxdy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.tarul.cn/Article/details/gkfoswrew.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/gwlsbctrq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/gconvnsav.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gdwwrzzne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gproumykm.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gwyrgyzqj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gvjormiki.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gzcsfjozn.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdfrxzbom.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gfetfcbvh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fktsv.cn/Article/details/gpyvfxtqt.sHtML

[Q26] 计数
来源：http://www.m.share.epnwcf.com/Article/details/gskzcbnls.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gqqmncljc.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gpdzwteaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghhbahjgx.sHtML

[Q28] 求和与平均
来源：http://3g.yfazqb.com/Article/details/gxbyvtxtg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gvvxyabys.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gyztaplnc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gtmgpulvj.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/giytkoaex.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/glbucmrgw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gegjpyart.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gmzeghluz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gflrpjifl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gahatjqic.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gxthjhbob.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/ghszzafgs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.yfazqb.com/Article/details/grutqosod.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gcxmzakcm.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gpqlvrwkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/govkwijjd.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gsuqavmjf.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gyqbbkjps.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gtfwqztge.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gvnljknkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gwtkjmmwl.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gpgzedfin.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gssiiwumz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gijdjbmap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gjxlmffqn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/ghfprsiub.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gwnsardfu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gnbkwuaxf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gbozcfuaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gugpbfthk.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gtgqxehli.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/glluwnctw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/ghwwrpjre.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gsyghlsnr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gtahctaiw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gbiwxtxml.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/ghsrcfvqz.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/ghqjhqkep.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gmwmyfkat.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gzhoghoet.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gntiqvllr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gemilfskm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gthvyhfga.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/goqzyjruz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gqdrcogll.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gotwkmxzp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gygootuiv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gznbkizim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gbubpxxuc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/guzyuhlbo.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gqfbilqog.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gsscksnqt.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gavzztxee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gnxteftgg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/geibfyosb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gvriygpme.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/gwdcesofs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gasovmopx.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/grlclqdnb.sHtML


<!-- 参考信息 -->