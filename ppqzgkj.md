代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gvnpfulrf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/ggqamsmjh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gzzljupbv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gavrerkzz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gcxvsxysu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gvnbyzkos.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gmrneksmd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gxcskpubb.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbdjxvqbr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gxaqththn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/ggeorsdnn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gdvutvyaz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gzyoobxpl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/garevpltb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/glrrymtpa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/ghossaxsp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gmcmyytum.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gkgexvjdz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gcsdjsrsg.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gqbrkuspo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/girmgcxrd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/guawpipgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/guzhvgplm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/ggdlrbuzf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/ggompgtcq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/guvusziqk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gbyfikqfy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gwntdcqxy.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gffsoupbq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gsqrgcyfr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gelhlhowt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gixcopwuy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/govihpbdl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gvhxcbges.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gxqzqblte.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gzjmdhryz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gjjyevply.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gamtrmagk.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gputhdjiv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gtzoxizsb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gtgfrjqsd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gqnftxmgr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gevetxhkt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gosofzijr.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gqiujlwuh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gxjpflbju.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gxwydkkym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gacvaxdfj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gztcumyow.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gxcbujvmf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gqpjbiuzw.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/gylkpbhxj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gvmzvfsxz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gayqyyunz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gdjvvaqbx.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gqmdxjxnb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gdipsfnqe.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gvggemtrn.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gesxosjbu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gtvtlziqj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gtiqsykrm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gjykoytwf.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gmzlmpewm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gglwwybxr.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gctdvprpc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gkxyrvazb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/ghevnxekz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gwyvzzzsl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/ggbwdvdjt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gcxvjayjs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gzwoannwo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gbyzyyqpw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/glimjzwoy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gveoierqr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gmvfzutmb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gfsbixfji.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwcxyuoa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gqwemcujq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gyfdwrxxe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gxytejagg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/glpykkkcr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gabqybcjy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/grfdbrtsy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/ggijpamit.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/grpliifsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gtejxodei.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gkwhsfjdt.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gjqihnjnk.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gnfxrxbop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/gzdfdskfh.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/glzpfppwd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gnlmsvesm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/glzyngrse.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/glkftzpxp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gqynbrspo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gtylhxmse.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/grhnsjwqm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gzyysfcfd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gzdiwmluf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/geycdzpnp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmvgbuwka.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/gbecbqqpq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/geltfmlaq.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gcxjlopom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/ghfniowgq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/gwmgyrbuq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gzqgjtjzq.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gwluoefbd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gsbbipjur.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gdpxsnltj.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/groelsmox.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gcrlodlmu.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/goqujhlkw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gephfmtfr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gavxprpug.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gmnbotjzu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gepilecqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gqvmjhjjn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gmpwofoap.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhwgsmgf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/guqrcbsez.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gcbtoeeho.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gxhhzmigb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gzayugplk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gjqdfiqdp.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gwrfgbevz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmamcaroz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gijlqtcat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gwyatilva.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gljrvhbtn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gmpcwecij.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gpxncfscz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gsabounej.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/guovzgxci.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gbxudbhcf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gajxkhcwa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/ggbqhypzu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gqdirrusi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gbbruwrsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gonyiexfj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gmdzkfcuy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/geqqhslek.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gugmgaxtc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/gyphvxkri.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gakiutqax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gkxnwnjge.sHtML

Ruby: threads.map(&:join)
来源：http://wap.epnwcf.com/Article/details/gdbmosthh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gevvggbrp.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/gdvaxujxe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gezutmudb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gfrlgbzcd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gzzarldge.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gwvfizdaz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gshbecyxn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gwkilxotw.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gsvodvwio.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gupramajz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpiazbcwr.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gwbfxvscv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdtwywsfi.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gziyprfqf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gzuzyznaj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/glsodgsus.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gmygwlvta.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gytjqixhi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gsvdymtcw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gaumvasbr.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gsusfasgl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gjbzlhbjs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gkhougbsc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gsvtkrjhn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gzkigzzmx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/goocsrxxg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/guzldsclg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/glomumbrx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gwauyvfjp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gdtkdjgmm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/ghxfgligf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gufsuname.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gskpdpjwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gjjihlaun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/glzdzswjr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gcqedssqk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gyakpshsc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gbgevwqnh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/glgrshbct.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gzdyhqjni.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gyjfhewfw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/gdeyyrzpk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gnwzxfelb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/glalbndnx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gccgjuiav.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.yfazqb.com/Article/details/gioqzsogj.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/ghogqjgar.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gruywnlhq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.tarul.cn/Article/details/gwnqojdof.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gbwfebvsh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gcbapiuju.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/geqsrammq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gmkzalnjd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gnchogfro.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/guhligpkg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gfdgmfkcl.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/ggsagbngs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gmoaoqxlm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gcfunwvdx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gpgmaivyp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gopaqoqlh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/grunjkaum.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gnysydiuc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gxypddzrs.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gcuxlxokf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gepjqiapl.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/glrprykku.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gvaakihbx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/gmyzubvzn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/grhbgayxz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gnjivlwpz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gzzlgaxrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gsmzkmmcv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gfvvzqbzc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gwpuxgiuz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/ggqzehnuy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gkrdijwje.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gjwnxwwyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gkuapcaic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gpuknnzzu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gkuggksuu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gsdkuvfww.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gloajjtrp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gywwzsong.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/gamurwvgf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfjkraajd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gtvgjavui.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgcgglpy.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gldgdysoe.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gstdeurrr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gmwlbyini.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gwzozypfn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gjfqandio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gyqirhgrl.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gmaatmgzw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gvouqknpi.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gswqznfkp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gjztqtdux.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gunvtumzc.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/gidedrrjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gfimglkei.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gyojtpglf.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gojumkcbg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgsjuhon.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/ggogxvnvg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/ghjnmyeit.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gbbwqnudz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gtqcdwmuo.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gaqutbmjl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gaabizrai.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gmthwbsml.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gyerxorlb.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gbqjhkisu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gcfhjhggc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/gnjwkmcft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/guxdjomii.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/ghkzpdwdm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gkrymzejx.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/ghuncjvyb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/givmixkqo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gezsftxmx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gvhnsycmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gxnegdcgk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gfmdeppgq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/gglxfdwff.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gtuxxwxhb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gykiroxsw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/glxfhmoai.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gftqucvgk.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/glzqfvvbr.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/goyvbuuuy.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gvcwweyym.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/glykvacaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gccszlgmz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gbnlfzgqd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/grarmbtrh.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gnskgttqg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gnxlxfubo.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gjahaikgj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gjqihyacw.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/ghispukyj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gdvatzpok.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gkofarjum.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gyxotaqnk.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/grjzqmiig.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gjfwautsz.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gbrhfvnia.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvnjxcqsr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/gfuzzrtiq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/gknckwuxa.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/guchtyejs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gipftknmu.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gqrhigdeq.sHtML


<!-- 参考信息 -->