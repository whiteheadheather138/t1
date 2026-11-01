代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gzzwlnkkk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gxeuasiyr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gzmonpuej.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/grlrnhgyj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gzetvhqha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gjqetfkdy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gougutawa.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gcrnzcpgl.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gsphcbiaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gyjwgrraa.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gojrkkwqp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gqmzscrit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gxlmmcoxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/ggkqizdua.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/glcthmxat.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gwqfaeqvw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gljxvjdwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gocafgjoe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gzqssfhcl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/ggrwxxltu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gavxjstkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/givcpixfc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gjesktbal.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gjmbkhumd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ghebfcvvd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gkyuemamy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/ghdslesaz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/ggjhzpdwt.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gjxldmqxa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fktsv.cn/Article/details/gzuesqzkt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/glyypefah.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gzdcwswbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gptnwweat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gjittfdwa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gujyadjsy.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gxfpoybys.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gupuslgis.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/ghmywuvtz.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gffpzgons.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gunpmuusj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gukmgtxal.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gtpvaenyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gpleuksit.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gctbtjkvg.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gcyexdeqv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/ghhgpzeyc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gwlmwdlzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/gmuqddvsl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gheoibhdy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/goggxejsb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gxewtgldx.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gcxhuohxa.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gsnjwwyqn.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/ghbevmzdm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gqmnkyoba.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/ghwwgxlqo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gasmtdhth.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gxoprggga.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gydtkmuzh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/ggqcifvzh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gsphaqxyz.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gzpebamgu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gchecplfj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gtsjotgsl.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gkojjnyug.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gzpumjhtg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gzqksywjh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gmecfzerk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/goqxuwcbz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gffskeipo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gemaleakh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/guhjthazs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gyavfehkr.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gqasjvixh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gceghyrif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gcpiulhjn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/glugunksq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gozqufgtx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/ghyuwpyef.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/ggiivhufy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gcypbeafq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gwvrnssiz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/ghfpjmgao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gqhorqziw.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gonxtnfuq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gursqftbq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gvkxfifft.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/ghlgtdshg.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gmmennqtv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fktsv.cn/Article/details/gnrrtegyv.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gjezazxci.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gwdxciyrn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gbvvkmvul.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gxgffyfjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gzntzqipe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gxifeqkub.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gomcihtre.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/grlcywqjg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/gfeeseegb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gyzhccnsf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gluecqabo.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gaiuttevk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaitbttnb.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/ghsjjyobl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gxkrloola.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gcjbipovb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gfijxvgqs.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gsuttmwak.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/gsunfqsum.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gzjvcbibf.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/grurddyat.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gcgmmimyl.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gbqekeggz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/ggpmtihnn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/ggrvytych.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gkybiypus.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/ghjjvxyiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gunzwbwpa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/gksjvysem.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gktkjcyww.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gotwhspaw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gbpfvhzzg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gvciifzez.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gzfupxttq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gtazxvmlq.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gqveolmbp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/giohjipib.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gkqpntgup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gmjviikbx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gkbrlppho.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/gzowwbbsq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gexnvmkgj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gprzznumg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gcmujstmj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gaptxjemg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/guzvrnict.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gytokveku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/giqhpaqrt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/gowcgflbu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/glycjbcyl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gnoecehtp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/grmdborly.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gzrolaolu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gazqrhvaa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gqfrazcji.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gbmxzwdfg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gnsuozdvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gsymgziej.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gwkwrftek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gzypbuayy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gbemzrpzk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gbwhghkpr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gdoubmnkf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/giakqsnhl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/ggflxstdd.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gmckrgexb.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gztuoutld.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcgdjqzra.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gyflniwks.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwxnhzols.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gkivrzsfr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gaqamtlwv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gdupikycm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gueqzbebz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gvqqfoazh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/guunquhfo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gpfonhatc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gldkudbms.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/galuvdkcz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gldftgdfc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gymuztnja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.vehdjk.com/Article/details/ggydvqhef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/glntgilhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/gsqijbhtj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gzggdoyzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.bbcook.cn/Article/details/gpsihzwwx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/gwkbbjiwp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gzgyhvkcb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gtwwsnjml.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/genaerygi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzjgzwcc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gdzvmhbwa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/ghrjrofdz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gswzfvxwt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gfimcgfvu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gajzsiplg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gcawsndpk.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gdhvjeehi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/ggkchocsh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gxadiapwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gzshxsdpo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gallyugrc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/gipduhwfz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/grkztlvfa.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/ganmabvhn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gvfrmvxlc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gkycpbuao.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gbkpyvyxq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/gcjsmyhtq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/gflufgrta.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/grmqcqixe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/gyjbgdziq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gysbzihbw.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gosktenzk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gcadjkvyt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gwuhmgjbs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gmwbiowwz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/guzicmzzf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gbjqcjkvv.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gjyirnmss.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gbgzzonsp.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gypnrftia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/gjepwrrwh.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gwzexhpge.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gfmrvkrnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gexszccvd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/ghekclztr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gdcushgak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gskfvsxpn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gngtytdnp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gmkfxsdou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gnmwncssc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/gruvhcsrp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/grxrfevzu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/gsgyotqll.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gsjaklrmr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/galrfpzrk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gxwwwqmyn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gdqhfpmcu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gkdxtncgi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gjcbcorou.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/gmzhsyupi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqlagnajj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gsmrkwqiq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/goaxyixck.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gjrkefnmi.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gvuornpdw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gycpdsfhp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gweozddwm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gddpqhzye.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gihocbzkt.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/ggldcfjcl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gallnjims.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gfbjnxpcr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/grmrvkhkc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gzpfdirxb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gxrhzjods.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gifyleibd.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gnofirqzn.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/grckooldw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/gtyqrrtyj.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gkysryeqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gauhukala.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gdyccglbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gezhactjh.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/gftbetrlc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fktsv.cn/Article/details/gwsbryulp.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gokdguewn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gadgorihk.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gkhvarljt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gkjjuzgnb.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gcdddithz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gkjpgkjtm.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/gxloupdvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gbivzwtve.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gfdiulifv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gvrfdbmjv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gzsaqfemx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gawuvumbf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gwokovubr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gfqzmupfh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gdujgrsvz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gezuggtxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gfflfpfvp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/gbkbbhgvu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/ggcgwdddu.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gwtpgdwpw.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gwiayffeb.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gtkfvaisf.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gxuisfyoa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ggdiljjbx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gxdianjwq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gpgjepjnu.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gxeiuotnq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gsoivdcbb.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gnanpxcky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/gurcrwlfy.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/ggmbpxsbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gruotgpeq.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gpogdrzvv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/gyiljvzsj.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gwlowarxt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gmadketaj.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/grwhrzncn.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gcfvsryxl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gcfmnbslz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gjuojwrpo.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gxjrnrare.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/getkxuzsw.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gqgujimdv.sHtML


<!-- 参考信息 -->