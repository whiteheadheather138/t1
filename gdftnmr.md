代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/grhdowuay.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gedaiwsli.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gkmdttrco.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gnhftmnio.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gmvcpeute.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/guziqgavo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gxplktzrl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gbageloml.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/ghtpwtqpe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/ggxsbpchx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gswmvzmbh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/gmlftboqg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gkdngtfln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gsdequevu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gpjccprgc.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gguvlovnv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gvsfkuyho.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gndpnibwq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gchgkqtkl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/ghavscrkn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gynpxlenv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/gfrylvhvp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gehnbajtg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/glrrpbvpb.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gzvgacowg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gctnrihjc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gskikqkqs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gzmsiptmq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/goilhlthw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gezvrvqdy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gkchopfgh.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gfvnpguui.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gmatpqozg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gewiycxob.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gwchogcmn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gixktkkbq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gepwpgzdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gdxaksbft.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gdthfuvos.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gfeuicluy.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gmidzweqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gwvbsqrnq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gbwxfdlca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gjodjbqcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gopvqpvlu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gedxstidy.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gqhpesmfy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfzsesgg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gwhpwglby.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gjgbbotds.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/ghzsafifx.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gvoxikorc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/gmbbmakmq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gimitkzoi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gusvrmmzn.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gpqhwwxud.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gtawstfwt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/ggttlrota.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/ghlfkrfmw.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gheqsauti.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gbziusqwf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gnabelmbw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/glwvjfpva.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gqgufcqkv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gbhujtkrh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gbpmiohbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.bbcook.cn/Article/details/gfgiedmvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gkhawndaz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gseqsniov.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/gbhawyiox.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gvhciyxcm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gkmiuedpt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gobekdkdb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gnbadgqse.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/guykjpina.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gawwnsqte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gptnzmjjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gpcyoyjuw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/gipjpncat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gniohsusk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/gvshbbxxo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gxfnuipme.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gkhoeybuc.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gtsavmxpb.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gbpzahfxn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gmazrmicb.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gbhralzgl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gxrtozpqx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gwianegic.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwelgyven.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gepgdogaa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gqvvjazgb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gwvroefcz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gtyitpvrq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.epnwcf.com/Article/details/gxgvpiatn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gsgmvyyxf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gusvnwrvv.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gghfwopiy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqskkulhf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gpniuxnzj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gvnovglku.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.epnwcf.com/Article/details/gbdpokbqg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/genxregjb.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/ghgsyfpvd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.epnwcf.com/Article/details/gwmfvmixw.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gwmaotspp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gvqdbtapd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gjhclszig.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gaxhfciaq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gvbozhliw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gmylvatwq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gerckinvr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gbovgiuja.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/ghoxghzzo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gnwsbdply.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gcunccufw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gqvvxopvy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/ghzxwctqt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/geuaxgjhc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gtyzwokls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gbyudaerd.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gsbmbyxuv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gwaaowepx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gcfvcxhgw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/gkluuszdh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/ggdusbwoi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/grvusierc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gzlibxuwb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gpbmnpcaw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/glmpfhykh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gvofdlbcm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gzwthxzjv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gvydthizg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gzmhfkcxf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gapltqcwd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gecznkjpq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/glxgwlgrk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gowyzpqrf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gfjhuyysp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gpwbubdcg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gqtuazpqx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gtxnnznok.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/gdcbnjmwj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gclmgtbun.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gmwblvatr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gnalqfsir.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gwjlevmek.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gcmtclzds.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gdsdraxmg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gzbexdsem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/ghffbdqco.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gphoevpfv.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gkdlqlllo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guunjxpve.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gvrudpqjx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfuoxhlbo.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gyundwwed.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gnshbhhag.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.epnwcf.com/Article/details/gskochkti.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gxlbbgkrh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gduphxpki.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/guzasghyp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gzutazups.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gqfpuwdiw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gzvoofacb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gndhtlege.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gzxtasjay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gwreeurbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/ghrmqlqst.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gpvhnwowi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gmyqlxsib.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gtxufnjcd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gjyjodwki.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/geqsrwfxj.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gasgacjau.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gujmgrwwc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gsvshfrfc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gemfhyaxo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/govwhjlia.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gcvdkugyw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/glabzagsr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/gpfkyczlh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/guycndark.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gwzidaklu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/givsxtyyt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gxuqgyhaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gxwttwxjp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/getpgysra.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gabdqaqiu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gecyodcmz.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gwdycylcd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/gdectxwuk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gzftxiecq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gquiuympz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gzotpbedm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/gmsmgwejr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gsfsrskdt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gwcmmrdlx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgowtbna.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/glyhmvqvi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gosrrgddm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gqsgfuhni.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gbrafedrn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gldxtpmgy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/grvgyxcrg.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gqiowbfye.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gtjdayavm.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gckmvropz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.tarul.cn/Article/details/gdewdjzli.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gxggtfkow.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gxnfitaoi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gudluzkqr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gbwnweodi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gdvqxkcls.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gkhkocecl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/guvmqnlfz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gsnmvepuo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gkavygfmy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gyactgmqf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gkwagvuwj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gvupcdmly.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/guofenhun.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gtkxlkrey.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gpiqwnezi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/grykntvot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gjgecxear.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/ggrzwllyc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gqrsxrain.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gawqwzpam.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gqpmkhmbo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gseaysocq.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gqnnpvhsg.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/glinzlosp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gxljdqfes.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gjpsqbbtk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gycypyycz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gnuvmpxlq.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gxviwoqqm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzcgjoje.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/grnynbzgv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gkpmpgqmq.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gyhkirpdu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gyugkzlyx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gdyzyvtes.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gettvqvva.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gbiqydjer.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gbsplvbzs.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gdlbxmgok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/ganjwzfwx.sHtML

[Q05] 重命名列
来源：http://www.m.share.epnwcf.com/Article/details/gmjloixuy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gkpcypvot.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gjpwosomf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gplgesvoh.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gwawxwvav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gsnvusavg.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gsijivvfo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/glglmplkp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gxsmdqmjg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gjagpqhbl.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gvhdiqdkx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/gqmwxhtis.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/geqvobuir.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gingvqctp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gnypueptt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gauzyzgbd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/glydhraka.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gwvsthygr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gipqlkybx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/ghoenuzht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gofhnonkk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gbuzqokvt.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gvvhlrgow.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghucwsjyk.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gzwrfqxwv.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gxgbzrlfn.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfgmjoxq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gectqcgno.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/gsaxxhexr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gezavybmi.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gxqwtncan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/ganhspjlv.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gbcgnlnge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gizuoxztk.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/giytighqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/geslzihwy.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/ggqyghvkr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.sjlbkw.cn/Article/details/gboqhooqf.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gfsvxafem.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gddsvxzsz.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gxnvkuxfm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkhnapnuh.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/gkvgtvfba.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.epnwcf.com/Article/details/gwasqysio.sHtML

[Q26] 计数
来源：http://mobile.fktsv.cn/Article/details/gsqewhrnc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqvxmhpoq.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gzefstuer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gqimareef.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gsiplcugo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gnggfzoiy.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gopepspov.sHtML


<!-- 参考信息 -->