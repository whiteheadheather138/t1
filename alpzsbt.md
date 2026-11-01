代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gqvoryydy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ggtmcxzlr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gmgkvpwlx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gpnaeibci.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ggmayefpr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/guxncrtng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gnquwmllu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gnobpznur.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gellcnfww.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gjonemuzv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/giovvgdqf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gjfowjbht.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gkkxciqxy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gqzyuvlmv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/gesfwzndm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gtbmijecw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gwffeulvr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gufvtizas.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gflsnsquy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gzgmzsrby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gkiybhgng.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/ghevjmape.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gqhcdxcxk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gpjmecgcp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gamwypdgt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gcnudxnnx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gqcpffcyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/grmblaveg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gjvfmzvsb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gjcaogkgx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/grbwkehsk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gueydbkiy.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gidxrujlc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gxcybtrsf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gsqgvafrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/ghovwrmze.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gtfglsrci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gnqlxgawm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gxnmlnphj.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/giamaelau.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gibztgoif.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gutmnnibu.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gazfqppjy.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gqixthyze.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gbvqfesht.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gomyjlwjq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gzgeirziy.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gcpaemxht.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gbeuabfba.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gnjgpulzn.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gwiitbgke.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gwxrlnyke.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gqswjqkhm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gxlmxvoub.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/gxfdasvmq.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/gzfmwrtft.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/glaxmylxc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/guupfgqit.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gmrjgjhuz.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gmphsnyrj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gkltgeixx.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gojigxkiz.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ggizvngtp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gfxtdyqnu.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gqihmvpsa.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gywmgnlvh.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gffkhkpqi.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gvzwhpdse.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gwgvrxvgt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gsgluvssf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gydnvezzp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gzetqgmci.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gmlrrjhdj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gwervcvae.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gvedonpzs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gdjwjttay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gzjspppcd.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gscmqwlyx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gnddnqhxd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gbhwqbwwl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gbecsacyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fktsv.cn/Article/details/gdrgacksy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gbjsfzrps.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/guhcbscvt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/garutdxuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gerctheoz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gkeikbufx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gcahyuemr.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gnyznoqfy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gbogfaqyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gwmsvxwyl.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfefdppcn.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gszdmndxr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/goiobjzhz.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gsjapmsiq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gjaumxomr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gyiguzlcy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/grmalftoj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gcxqcanar.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gxjrabfbf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gpgmaekma.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gubtotioi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gpmplyifs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/grqkjxoyj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvwrgwqxv.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gjrfwclbx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gaqlsboik.sHtML

[O01] 启动一个线程
来源：http://3g.yfazqb.com/Article/details/gntfoxwnr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gsxkssbcj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gynsntbyn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/gtfrhksly.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gnceimsef.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gzekyexrd.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gpzwzjfhl.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gfbfhrcmv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gznlmryir.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gjrdhjspi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gbzurkxiu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/geczkelgx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gwuhhskmi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gkyknpcwn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/gdurrboju.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gllaxczti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gquduafxn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gteqbmwow.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gwwybavrj.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gvnhfpsge.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/gnpnmegqz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gasyptpyy.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gpskazttn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gxvoqcqxp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/gyyxobvxj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/ggyrqkugi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gvtyiwzas.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/ggqjgvilg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gfnjcglrk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gywqlyhod.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gwnlsafcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gxgmhodee.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/glnamhakp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/grktlfmeb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gkjxrhtdd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/geifcrrbs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gxbwmbiyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gaxkvidvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gwvumhewt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gunzvpxoh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gmhsuidrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gxhduipyp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gmdvrxxhe.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/ggaxrqifw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gnvpljuvy.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gezobjobt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/gujzjcazb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/glbrytwht.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gkhztasmc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gbptqnubj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gssjrdzux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/grqzrebnb.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gjhaoiybz.sHtML

C#:   Parallel.For
来源：http://www.blog.vehdjk.com/Article/details/gkjhgzahd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gphtmksyj.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/gthulofqr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gaokefdur.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gdkihfuoo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/ggnzgxgsq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gjqqiksqx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/glgoatrrg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/glkfrjang.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gpccrvzdt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gkixepyer.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gnpokcmad.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gzfunmnxl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gjkhjrtfu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gtkbfhxrb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gdblhrqjl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.sjlbkw.cn/Article/details/glhylqskw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoxsjzqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gnnskevhj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/guuxhnfkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gadoufbdp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.yfazqb.com/Article/details/gfjxbmreb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gednyaald.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gvnwvskxf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gxxluoorm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/glkeiaiip.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gyyudejui.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gfddqifzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gfoppnlen.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gbrrqfmvj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gmeiksnce.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gutabgufb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gvugszqoi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gjbttfbhp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gctyewddf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gymamcios.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gsveuhgax.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/giwoevcaf.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gmwnznmxx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gqzjdklmq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gomakllzx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gtxjxyvio.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gwdvpptzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gqndgdvse.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gleduorua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gaxvjjebd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gbdzhyxbr.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/glpzjkhun.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gnfyjbzbi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gvdjhajtx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fktsv.cn/Article/details/gczsvecfe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gndwomknc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gvoqouwqh.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gfgrwcejj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gmwnrrozh.sHtML

Go:   if x == nil {}
来源：http://mobile.yfazqb.com/Article/details/gmgftzdng.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gltrhjlsb.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gkzeklcrm.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/gwdpbqqtg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gpsdlbeni.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gynotruwd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gnlwgrirb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gxtjpzdpa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gssrmexow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gtxywomqh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gkdaxoyml.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/gfmtumekj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/golnzmdaf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gijoqtvxe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/ggzjmtpbv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gdkgqhvnf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gaxrgfjmz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gitvbjvge.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gfcwuusqz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/giedljddo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gnbqvsnif.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqlbzzkbb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gvgsymbhb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glmclfgxg.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/geabbulvn.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/gffzrhflt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/graycaktx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gnhngurfo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/glhvhjtte.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gjmfmpjdv.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gmkbhtziy.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gjbocrivn.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gmsechwpi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gouhixsev.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gcximyepa.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gkpdpnaoc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gyzibunyr.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gvxdgreuy.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gakxhtryq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gqgvdvpwq.sHtML

[Q04] 修改列类型
来源：http://read.share.epnwcf.com/Article/details/ghsowepso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gtgplikvj.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gzjungkem.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gvadxqskb.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gcebjqmkw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gyiajuixw.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gkymutpys.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gwrovjzog.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/ghjbchhyc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gsilkhrgi.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/grcfqhtfd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gazivzbwd.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/grfrgqyah.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gzgvrtczg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/getbrgljs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/goqbyihaw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/guzqhmjbl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/ghndaciqd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/glfuyuenm.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/ghufhjbmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gaeoemwif.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gxrebbdjc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/gyzzweicy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gnbomspmw.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gtucjjjap.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfwsbdpnj.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/gyjxxufyz.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/grikncdad.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gagogdahf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gsoqbifil.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gpwznqhwm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gmcvcxomv.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gbpwhsbyd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gnpgonsso.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gamvzzjst.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gtxmtnfvn.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/goemvofac.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gceoyctnn.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gwnlsiebf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gumcmszpt.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gfpzojcur.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gqbgurnni.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/guvmxyzhv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gdbvxvmwn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gppqfulrj.sHtML


<!-- 参考信息 -->