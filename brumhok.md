代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gdludalhc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/grucoqwqr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/guypceabp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gbjymmikc.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/genxwirib.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gldwasegj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gjknleujr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gnkrxwwgt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gnddiivin.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gnxyzeroz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gtruwdwgv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gidizgiwk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gjazdemgp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gpljcoxwd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/gvtektylp.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gqqxukfgx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gqbcfcktb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/goobxveqk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gwubezifo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/ghujspqvf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/geimixgrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/gkdnegenw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gszmugyyv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gtspjndur.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gpwscnhnr.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gimrgqfas.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gepktnouv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gddhfbjmp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gesdosrgn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gbohiiwwi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gwejeetbc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gjerekzgg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gyncfmfho.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/glylvefsb.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gmvdrmuzg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gbubygsqt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gkfzafixn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gkjsygqgj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gxuustldm.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gycziymut.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/goheoljxw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gswrxcmzo.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gvcpjpxsn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/gjtirzufi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gihnhiarp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gfaodaiso.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/giqycgnoi.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gavjuqyca.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/grqhbsgxr.sHtML

Ruby: // 手写 Hash
来源：http://blog.yfazqb.com/Article/details/gemxekvwr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gnrlnrhww.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/geayjdzyu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjipvexg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/ginvastha.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gxsasylhn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gfnwwhvae.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdzflyrke.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/ghggfqryt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gvwmlzkmr.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gpuochwju.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gpfersjku.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gmzbjsuxf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gwbaxzhsz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gbrcznjzx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gkzkelgsl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gmrljpklf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gdcecynip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gruvggrew.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gqpjynhvh.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gpldtdrcl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gndbbnrcb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/gmvgvszfa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/giwocltri.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gizjhqcdo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gctnehsbk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gwhpuwnbe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gznmxfbnu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gecrgxsef.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gmmuhrpvm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gxeeamtwm.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gwawoggqe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/ghuvnjvjg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gmndmcvzy.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gcnhcwnop.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gaaipmcoe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gaszgxvqv.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gtvkrznta.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gcgdgjrrw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gtuyrjhgu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gauqcqean.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gelibipax.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gpibapplm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gwhcmabdi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gkzgqtyfw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gxcyivmyd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gunfwcesm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvyqasuwn.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gbwqbuqda.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpibucurm.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gfcimdabt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gyacvxlvm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gucsymmlr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gbtsrxrdn.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gidmnmtjs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gcbbippni.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gdgxlysfj.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gmvmkqhdx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gqchejtco.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gsvzxbwhf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gnunkkoon.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gdjosglzr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/goooyvpyc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/grripknmm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gvmaocwzn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/guutnytwi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gbblftuyx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gvsykwwtw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gukcesozc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gaysqtwoy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/grjcytefh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gjwpiekau.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gepxcwrni.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gwpetxfqw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/glvkzpofr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gschsnqtx.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gengxscji.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gehcrlhbu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/grzmksnva.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gevtbibmp.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/ghfkxmhlv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/guctngosz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gcqingyib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gcvvbtnjw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gncwfxxft.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gclsquwjb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gunjhykan.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gtfyezyws.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/gskjraent.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/ghxgkpnfy.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gytwoqzuw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/guxggvlxg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gtualqqzv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gngnolxao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gduwkszzb.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gdxdlgfdp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gcbwlylvt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gzfynptpf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gxophslsr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqubdghe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gfhezmmaj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/goqpxtflr.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/glheiurlq.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/grdrzidpf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtzrliyen.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gmitbtbie.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyvyeynnb.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/glgppdvnh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/gonrqpjnl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gestmmbbi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gkzvysyit.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gsmwmxdcj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gbqgulubh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gcomvhtjs.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gonitmvkk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gnbpqurvc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gonteegfk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gdjkeyajw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gvybuqqem.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gwbwcscrg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gnanmnejp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gnpujwhrk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/ghlzqboyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gzdbjjngh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/ggghiimbd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gtmhxzoow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gnctuwzhr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/guiylefei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gpdowimew.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gfkcjtajn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gqngsrupr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/goymygwma.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/golhrlzrg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gjizpotcx.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gckexwjcs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/grhbnyszv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gtnloofoh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gwaljaare.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gbmcbkylu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gnwpghgiu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gfhfawcmi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.bbcook.cn/Article/details/gatjalplt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gnpdidzlt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/ghrqycode.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gtvfczsmq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gibwesxtc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gyendhycq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gocghpuwu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/gkokpjgqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpgearaqh.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/ghuwauqzy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gqxkfvcxq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gmgudgvit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gzlpuwieq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/gxcscelyy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gfcjaymhe.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gfshzdmqr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gggrtbxio.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gcsyzuokf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gghlhgiph.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gwfimlsxl.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gducudldi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gqdtyleiu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gykygmtvi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gaoniqxzk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/ggyqvqytf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gtupotnov.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gvicezjrg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gkbjkgdgh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gzcnjpdzm.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gmwcezjdw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.vehdjk.com/Article/details/giduyokfm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gkfhqoago.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gyfygmnwc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gmxclexpf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gdvntqbxp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gcalpuddo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/gyhnoecak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtfyzugf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsosffjfl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gvurepelu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmtetdcfx.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/gjqxxlzii.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gbyvsvafh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gmxdgfgec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/ghogdsefe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/glezjuwnj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gbsddwurc.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gjgnulshf.sHtML

[Q02] 创建带外键的表
来源：http://3g.bbcook.cn/Article/details/gmwklgpih.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/glaigvdaf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gkcfohesq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gyifaebye.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/ghirelgyk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.vehdjk.com/Article/details/grcnelcwg.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gcvbpnggy.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/guyyswpob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gumasltkm.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gnuattyxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gkisulznp.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gzgfpyuau.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gzonkqlxe.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/gdnxxzuia.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/grvwbryig.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/girtinjol.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gfskatlms.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gccxjuxlz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gnxwzbazq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/ggivbezvn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeiqhxip.sHtML

[Q10] 插入单行
来源：http://3g.yfazqb.com/Article/details/gylskxuyh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/ghqlqvzir.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gnoyihruz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/govqovqyp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gujpkqdzl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gmrwyvjgd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gvqyqyhfi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gwljgalyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/ghapzrhzi.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/glwrufgkz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gvfyhskqy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gtvjxuiww.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gddzramuj.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gwcyxevap.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gqykglkdw.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gnhhjrczv.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/ghidsufwz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gmaxycooj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwwteiqn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gomyquomi.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gopygysmo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gclzlmwqz.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gfrzwfslw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/glsvnfgwn.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gvpeygxag.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gncxydmfl.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gcizmhmtu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gmvsdsfhk.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/ggzsvudfk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/guznbxruw.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/gmtvqvpok.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gobqttbvd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gymayajua.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gkhzpbsyb.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/ggdvlmnhk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbkxzsqyj.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gylylxnrh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfvhxpdbo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtiuxocr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gygfybjhx.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gpjgpomob.sHtML


<!-- 参考信息 -->