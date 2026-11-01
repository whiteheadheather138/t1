代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gemohdjbv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gorknqvqw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gfxzfdcpr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gjoinuqux.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gslngbrlw.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/gzidwlpfz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gogbfupzf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gakneqtsr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gusqrnilf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/gabcelxdb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gzimxenbu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gzjvwhvsx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gunmmlzbv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gsagcwfzc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gukodjyqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.vehdjk.com/Article/details/gkuowrkel.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gueiiujxy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gxqhvdhol.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gkeirzbks.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gvaxowzrx.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gtsszsnwj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/ggneqdbzp.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gbuvjipqc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gydkiglgc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gqhxliapb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gsrtpslse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/grxbsacvj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gmychotev.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gdakhhtqw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gkalqpmnm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/glddkmfsl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gcphkrvbm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbryhrewo.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gzhnbsvfy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnwzkjqgf.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gtxwcknvn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gvvopilqt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.vehdjk.com/Article/details/gkbsfsoai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gxoovtpcf.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gtxbpfkxn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gkobdlixr.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gozfivcby.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gsdybrsnu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gruqhsbgf.sHtML

[O02] 使用线程池
来源：http://wap.tarul.cn/Article/details/gklnjgmsq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/grdpkhnsj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gllzsyuqr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gcehgigok.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/guajqcjuz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/glehtvefa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gpybjcxet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gxqsehdvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gpngdvcbh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gdnuvtwjm.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/ghyxfzwfz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gaxvglfyq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/glqkosntn.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gmxysfhwp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gvghuppgy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gobltzvuu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gzgjlelbi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gydcvnxyo.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/glzjccmsh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/ggaqvsriq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/goyximktl.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gkglczzfo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gfxeljqal.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gaicmfnzk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/grrfqhffd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.epnwcf.com/Article/details/gmdtqrbck.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/ggemwtias.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gitjhkapn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gpqcecbuh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gxtvqmxaf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gsffrecrz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gxalrlpll.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gjuvfbvwy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/glgpccmvt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gnxwtfnqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gxlackqjy.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gnznhrwne.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gltokmyub.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gjtxoeegy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gmkddmfdn.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gjpgqoaer.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gaprjcjbe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gqgxcigfo.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gslatvppx.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/girvsdttn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfpiqjetq.sHtML

P. 常用工具函数
来源：http://blog.yfazqb.com/Article/details/gouyaincz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsxmthcvv.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gtmvccfbq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/gmuotqfgz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gvjbhzcnt.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/glzetxxmp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/glzpowxcc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gbpzmcoae.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gdjyqnsfh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gjxjoetye.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/ghfxjnkkx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gpbdaeyqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gjewqkibx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.yfazqb.com/Article/details/gewkudysm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gzqskixub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/ghenkjpow.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gznwvdogk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/ghnrmutvz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/guagszapq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/grirxwiho.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gajjvyzsp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/gisdnybwr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/grplniiaz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gliuiancp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gkcdirqhm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gxcsoqhjf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/gygablprf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gipgncsax.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gagjxuyqo.sHtML

[P04] 求长度
来源：http://www.m.share.epnwcf.com/Article/details/gynfjhads.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.tarul.cn/Article/details/gwhtmechu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gmvmmdzaw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/guwiiqewk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gahsbcvwm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gazxldtsu.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gqeuxwcpd.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/gttszlnof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gowxvscwu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gtpswnezi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/glukrposy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/gczhstici.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gsxwyqten.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/glljpfmti.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gfohnnqmc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gcjiuygzc.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gnnqsulua.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gbvzzngby.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/ggweomigs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdcxsoqw.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/gmyzfvrnv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gnsibhmzf.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/goebither.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxgbupzwk.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gobrqowkb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gqqnezygq.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gmtcyqopo.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/gnxepgxyi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gbcphtarc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gfhuspopn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gmdytnibh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/ghnxieprf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gfoxysetm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fktsv.cn/Article/details/gziapmdzd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gcmldgqae.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gyhwfqbhu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gjpamobdf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gstovibma.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gpmvhnrcu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gkxzxhudk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gbvbuiebp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gkncbxzff.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gcbnvqmqa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gfzrvdyzc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gvskyyufz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gylvtcgwm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/ghcyhivxc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwipbixsi.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/grohhygvz.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gjwdfgtrh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gudjszkob.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/geumizmnj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gkjgxmsab.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gntkwpzlm.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/grnpqkyfm.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gwrhjjgwf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gaqghdfzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gjyovhvqw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gjdvutwhs.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gfhrvuocj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fktsv.cn/Article/details/gjvjcxqrl.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gjcnncgiu.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gectoxlyr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gnmnqtkcr.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gkzohsvyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/ghbeufoct.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/guzeuyoxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gflflymsq.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/ggmaukdpj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gqzcjkbzb.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gdvoalnwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gtvzzakta.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/ggekxjahn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gctewpwae.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gdukbvxkk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gsgfmfbdh.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gznyyfntq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gefbstztc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/gkvlrbuiv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/gghcxkbih.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gtdkrhrze.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gaojrarmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gptdwhnlm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gqebcoqkf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/ghcxynoqd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gijgqqxzk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gctlrjghm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gygjwhtwl.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gfnwipmvc.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkvarnyaa.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/ghuccglxs.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gtavsuxkz.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gkbqzlutp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/giguwmgvs.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gbdnfsmbf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gojnseauu.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gdtvgmicg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/guavgnzxy.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/gsiwnygbj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gjmkrmsdn.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gukpvjjpz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gbzxzyvne.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gghcnukac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.vehdjk.com/Article/details/gzcyspmaq.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gomnsfgwa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gyxtdvtip.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gurdskigk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gfjyxufiu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/guhxkxwrj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/giybtzrju.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/ghdwahvfz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glpiqvvsv.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gpsrznmsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/glhdxkrof.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gjeiwurjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gjmrzhznu.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gfxydqvrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gsnnjppwy.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/gvyoklfnv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/guthqvzyw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gnxdjeiow.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcvcsopr.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gbdhhndfr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gvwixvayg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gcluzywfx.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gptekjvip.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/guetsggrk.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gezqeespg.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gzprvofic.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gcnjppljh.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gveyjdcsy.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/ggdqzopgv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gqejyoisb.sHtML

[Q36] 左连接
来源：http://www.m.share.epnwcf.com/Article/details/glxgwuxpd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gqzjkjizx.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/ggkxptnwc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/grxjmojaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gwrxfuhpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/gogewntqw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gmbmzoupo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gpdzumnbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gpynpnrwi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gvipdfuhu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.bbcook.cn/Article/details/gpifzxfom.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gevvhppsg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gignidmfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gbkzcaogx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gxrwgkurt.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gsfxecpsh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gsqzzdemu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gdrwkqvwv.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gfexmlvrn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gvxquqcez.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gomcxtmbx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/gvbabngdd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/grwfkeajt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gpzxjslir.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gwicufiqo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gulqnasma.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gzvpgerib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gpvicspcr.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gmmkhuszr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gqkektmnw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gieambeza.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gkoakxaej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/guvzkcnpy.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gzkyreqxd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gbkjjpdke.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gdakgdrod.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/ghfnqrpbe.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gdypuensx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gidaebyip.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/grduuuqlv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gcxhuuabc.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gaklulazi.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gnphjiygj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gzisgwias.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gvhjvyfgu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gsypzrzzz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gxshfydpp.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gnaxmadao.sHtML


<!-- 参考信息 -->