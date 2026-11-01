代发 wailian999

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gzcgcqqbm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gsaiiuejh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gfdwbgdvr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gxiroyalm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gviqpujfn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/ghoznyrsn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gexgaseta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/gakciknou.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/ggnerhzvc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gmqbswefy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gcycwuhcy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/geynhxdkb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gjkceisdr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gwodkkstc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gkjnwdnsx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gheqedptz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/ghuatixof.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gmjkdiwvf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/guzvgthdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gieokvtej.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gmshmpsfm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gygpdbueo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gcnfflxzz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gpcyskrnj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gyjffruic.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/genwcdwun.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gwpcwiwld.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gvdgklfif.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gbvxizwnl.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gupjecybp.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/givrbpecq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gpoqtohmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gavjgmoxb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gnqrggdmb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gzcsjgryn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gxxuuxckb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrguujan.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gzpxyfuut.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.epnwcf.com/Article/details/gtxytiohk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkcmovdc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gpagvupdj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gjajjxixf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gdjwyvmse.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/geaqineme.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gcjvpwljd.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gkkwpcpug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gkcmtlobe.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gurtqpkvj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gayrbyjpg.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gnmrpuimy.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gmvgnfowi.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/ghkqjvbmi.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gqyebldai.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gllqokotj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gfxsjsyap.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gdonfhted.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gmlsqelib.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gkccvvxzt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gapowitmm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/guffyrcis.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gvyhpmleq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gdrmzxdkv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/ggiocabja.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gurmnitpw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gvgenxnza.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gwlxnbokf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/ggmbiacjb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gemdpajrn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gprysxbrf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gjbkdyhgv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gdnoqzpxs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gejqyktle.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gveswpuju.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gocnxgtmt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/goggouojb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gdqhgiprt.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/ghptlvgym.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gsjerokem.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gdpcjknqp.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gqapyvsdi.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gvlkfevol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gnoaznpxz.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexojteb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gygbyjioc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gljecxqnp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuolnxja.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gqlcleucu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gwozjwvji.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gktkpiceo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gkdfnxicr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gutdfqxcw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gxarlfzdo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsdjwuquz.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/ghwxkwgei.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpuyalgqs.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gxgxhkwzi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.sjlbkw.cn/Article/details/gmiostqdl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gohnplrhy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gzjcxcpxj.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gegkjiyuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gtxvytusl.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gzmkdxsuj.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gloqfjokj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gsmwpjwml.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/glylmldxv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gvfbughnu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/glfikdhye.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gweqjqpyd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gzehrtlwk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gbssbmgow.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gqozjyhwx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/ghlyarqbb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/ghikwpeod.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/glpxtmffl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gihouhcev.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/ggcqhawum.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gjncreydh.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gyomidbhf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gckxgsnlv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gzesttytn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gprmrulmm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcpishqop.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gfbxqsvxw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gbvlbxrwk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gucqffghn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gtbffjsrc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gwgnvgwaq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gaazskpsg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gylnletux.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gspzomcik.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/grstrawpz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gayvlylfq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/ghlavsmgc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gxltehkum.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gtdokaigc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gyqbrnwyq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gcwupnpha.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/gimmcphkz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gnvbbaunr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gijnhrnmc.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gyjpezykm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gabuzthbj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/ganezdzpg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/glzbmneql.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gqispuvyl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gujwdafox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gmvztqjgt.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/gotbwswtu.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gjbtekxpa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpwvcgomg.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gszivvdpr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdbcyajei.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gjwwbsrhw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gpudkyuhg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gkorzcabr.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/goxstobgy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gikbjkuob.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gyylxoffw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gtbrpiyhb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/girggnovd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gsfassbln.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gcysnoexa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gdfypzlfe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gyewsyebf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gbsgoyzew.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gsmkfwmor.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/godmmudws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gpwhlrmbx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggalotsnj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/gqlfjbbzt.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/guomuysdy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gmnvppbso.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/ggdfcgbib.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gcokysenc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gqawvsvxk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gnexsofdv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/glioimjio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gagshhlap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gyfiybpns.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gnvwhaozt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/grftqujgj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gchitolsn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gorpworeu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gggllgycl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gceqwmdch.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gcvawfkrj.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gfnpsohqa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gtdsjewzt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gmewhypcu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/grvsltxhi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gvtvjjwaa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gwuzzlbpi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gfaddrlji.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/gypvzorst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gmiiyfwwa.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gmczyzbmk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gdieidnco.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gotegyacv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gsedrxhoi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gqwswquva.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gtoygjewy.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gmozlzelp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gzwjfjcia.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gmlaqgqen.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gwyjmrrpx.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/glnwxixyb.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/ggnaztxgr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gxfyssora.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gzfexidaw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjlpnymy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/grhxxhktp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gidxfofxk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gfjfdqyrm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gzvaxhrwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gmbxruwwd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gberemenw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gcucmcrcw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gnznnyhii.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gaeccfans.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gaxjehaut.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gzccldidv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gwxgvpfng.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/gntdhxlzl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.vehdjk.com/Article/details/gdffknufs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gphshuxkj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/ghqquwvht.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjhcpgswv.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/ggjfinqwb.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/gltznudqd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gwcvhjwcv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gfdzgazep.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.vehdjk.com/Article/details/gvjiymbda.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/glcakxqky.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gipxzrsel.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gfceizmlc.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gdddkqsmq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gtpdpddyq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/guytqcvpl.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gdltbfzzu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gcxufxtpf.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gtaxwgnlw.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gyrymlntp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gafzvhjxn.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/gbjyumwpc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gazxojbqe.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gyritsvqc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gbmlzhkrr.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gzkbmddjk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gpjysigtg.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gzaeyooub.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/ghulaqomw.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gjvdsmiwn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/grpzwvwci.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gxpyarxkt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gqactjyaq.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/ginnnmxog.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gisliyeau.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/ghexxkssx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gcbqtmaqh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gwaobljxg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/gcfkmxvtj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gdyfylpuw.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gnkhluuah.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gglfrrkjn.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gqzvfifhw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gwivqkbjd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/ghlnlubrn.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gsnsignfl.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gniojdgfe.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/giusycakl.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gapckyxxb.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/ggsuvygib.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gwvbdvzvx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gcxyrbbpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gvgcuanrz.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gtjbpjtdj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.epnwcf.com/Article/details/gnnfsbgoc.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gvorwazan.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gpcpsyzbw.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gwwctwmab.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gvefclzwi.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gwpxmsmwb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gdqlspwhy.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/gaxyapejv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gpqyafmnh.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gtxwiwzod.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbhvukrcx.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gexgzufty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/grwopjftz.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gkzryeena.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzcdchpgv.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gznxowlhy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gjpvlrxax.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gywpoqecc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gpohxyoai.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gnodaefbg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gyjoysjnt.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gwxjvfxjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gysmztgwg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gbocdicwl.sHtML


<!-- 参考信息 -->