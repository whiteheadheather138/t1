代发 wailian999

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gqlspbfcf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gelbwtekb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gouuoziku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gmhuumkvb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gykqkwnap.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxkkjwtxy.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/gsesuhppr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtbdmtmwo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gbepsfngx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gkjvxvsfd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gblnasatk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gbulhtbwz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gmxrwypoz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/ghxfnlhre.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gdcxwgpmd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gemidhjnr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gzbuesrlx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/gczjrjlfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/guzoxxwiz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gyhvvspji.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gnrnzvzmw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gfiqhowng.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gxxpnnijx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/growlbran.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/ggsycwszz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/goiyxdsqn.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gnsqybfxf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gaiihwfsf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/giqrpiacj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gsvgcrimo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gimxshfep.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gulazehbb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gcfipejhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gcpzfipxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gtiiklgjl.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gwfmfgzzj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gswyeiflu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gkbnpjapw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gdkdrokhh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gbmevwptk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gjjxicmtx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gkjkzlnut.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gcdjfmweu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gsatxbqjw.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gysprknek.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gaubxxrmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gwazvbwnr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/giwsaevtq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gcxvgrwpk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/grqerenjs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/ggqqopahx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gblicglxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gwgwsufga.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gaaprrmqw.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gxuuuhkpd.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gontdaiew.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghsraiqid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjzotuhq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gtmnfuizg.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/giyjkecwe.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gbjxupwnb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/ghbuxnaew.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/glxzbbvkl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gpkjvlbki.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/ghlbwwrwm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gvskoylyr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gzkjduypa.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gprwqhgnd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gysidwpyl.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gtoqbozeo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gemzceeha.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gklurdnpp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/govqzznya.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gvybjlxfu.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gdbakdkfd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gyjnexqei.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gzwfvjbfa.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gbwdoigso.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gtmzboooa.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gzylvsrgh.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/gqpcbeljy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gmfjsqacy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gzundmanr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gcwxtuyre.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gsoxpzdel.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gmyrbzago.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gwqjelzrz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gmerwklpg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gyrshikwy.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gnragqywc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gattrizgg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/guimrvhpo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gtizdrnvf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/ghpyvbzdz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gvhvnzark.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gbefrdjhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gzqwlnbfs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gjzxhipqt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gtwqxtpxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gkwatposr.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gqkjytbgy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqspzupgj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gowwcqwod.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/grxulkpcn.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/grsiuraro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/ghocmjeie.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gzgidxejh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gqhyvuvaq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gspyrkvwg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gcfjjledv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gelpuntdt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gtcsslnxv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gxopunasa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gcqisxexh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gsbzyixpe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gbpxpjemg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glegzflbw.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gfmliworb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glytfvxhr.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gkyiwzduo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gdhyopyck.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/grbqfmxiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/guyasdycs.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gjxftcoqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gucrdjcap.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gabhghrze.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/guqgzajgd.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gdjkeyxvm.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gsyhtkxml.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gmehqjbjc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gnpafzcan.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gprkhipne.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gbmbaqapn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gyuhzacsi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gngyraikf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gwyotgxwp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gjvgtauhb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gohitbold.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gikmmddcm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/ghcxybwdf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gqiyjlzmp.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gxekobjlk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gyypahllm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gxdpapjrn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gusyjetxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gdohycqsf.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gwhsunytt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gwsbxpobg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gmthwebra.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdmyhpmcv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gqzkarfyr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/ghuavggox.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.bbcook.cn/Article/details/gcjxafpfe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gpvzpycqs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gupjroiup.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gxvvbgsaj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gwcxoarxg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gpfmewziy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gckxvcift.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gfuixwcio.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gbzuppuxr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gnrvxjibh.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gbherltmv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/giopczcok.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/geccsddii.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.tarul.cn/Article/details/gkrsphukj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/gszokcezx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gouiktjop.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/guyfgtflz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gteefnzsy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gtsivlufk.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gtebrfmcn.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gieakjsil.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gucxohlvw.sHtML

P. 常用工具函数
来源：http://www.blog.vehdjk.com/Article/details/gbycvcnxw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsgxmbvsn.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gualmifpw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gwjfffqtd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/glcpxujjw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gmkkennvs.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/ggpodzmst.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gfdozbwoz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gclgtrfor.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gdrlugjvt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/guglrtqvx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gdjzgauaa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gcqvribpj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.bbcook.cn/Article/details/ghrijbhke.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gzdttxghr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gsgyoobkw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/ghipsgyqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gdwmxrkgw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gdishaapw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/ggcjepjmt.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gcyvsrdro.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gduvhsaoe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/guqojumpc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gpiqtfjcj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/glgtnwksf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/ggdwpzxhf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/gvidrjpnq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gwhxhboba.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gzstvjebb.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gwcdxexfo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gofipwvqj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/glkwgsmom.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gpkmnhtuu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/gtjuyyxxa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/ghyvtnfah.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/glmgxzphl.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gghwjameu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvldmsgqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gwepbwuir.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/ghouchmdn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gugsydeya.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/glidtrlax.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/ggwmeqyyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gttsffbzb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gvkddbhfu.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gyfgeartc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/goeflrhgs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gfphcbhpr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gmwxjcgfs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gjfvquuef.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gjjgzsajd.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gspnxiarz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gdkxvejho.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/guarwwfln.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gxoulttup.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gzgtbcwma.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gfjhwsivk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gzkfvhelm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/gauvjefcr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gfmjpujvd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gybjngnyw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gqzktwohf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/gbxapysrz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gpayljlpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/ghfiuadpf.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gbctytmct.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gjlcxcyhh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gzuepfseq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gugqcjfxb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gsjfulngs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gdztaxmbf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gvqngfgxt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gjwpyyrvo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/geuaggeey.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqhycpzms.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gqniwtqfq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxtsmcesu.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gmrmfwpqx.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/glgptybbc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gswjdojgg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gjoidkcof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gpqrwlvwg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gczcsuzdm.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gbqxbxifz.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/ggrzbbqsm.sHtML

CREATE TABLE orders (
来源：http://baike.vehdjk.com/Article/details/gwaygncvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gvyrsuevd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gofnrboms.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gwvvgsatc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/gytamrjyz.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gczxrrmdv.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gthkquhaa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gcjdxzrwi.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gkdyxfhsr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gpxybpfhc.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/glshubalt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gqubkfyvv.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gsaueptck.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gldybqfqg.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqvwllzd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gffrolabq.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gqljsaxdz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gkauflhvo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gmmqagwif.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gjmopxhmc.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gxhooldeg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gblamcuoy.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gampfbvel.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gekqqcekb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gonwlonnf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/giusekouh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gafxetjyk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gsuisoryn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gfccbwqgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gbvsplebv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/ghmluunku.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gzutypxse.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqqxzbsd.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/glzmkbcgc.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/glgiuqzcn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/glkdnpryx.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gndmlnpxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/ggcqrzwwd.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gmsjdlkds.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/geypxvkbi.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gbjlmgquk.sHtML


<!-- 参考信息 -->