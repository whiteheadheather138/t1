代发 wailian999

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gvioqfntw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqirhaxft.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/gzacmqczj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gspafzpju.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gxohqjzec.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gckwaaozv.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gmcfsjslx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grftilvuk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gmffciqzm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ginjsfwtl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gaqszqqko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gaahcwhke.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gtfdelfdn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/glhmsscvs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gsxkdvupm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gfoaetkqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtptsnzoy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gnokxwfkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gvzitjxfj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gvvcbngrl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gbqciqcmq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gpidwilxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/grdwhsugi.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyjjlcuur.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gdbbeqzyf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gjuadwgjl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gqyhofqdp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gkythguoa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gmttmkogl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpqlzpnd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/glfzmgoev.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gfdrehybv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gjmuczaot.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gnfkqteti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gnoesrpvd.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gbeczjirj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gzbqifvqt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gpozzepzj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gjeyqtknh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gouourqmr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gjdnplkwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gsgtnwcxi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gwygmonha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/giyoyohbb.sHtML

[N05] 最大公约数
来源：http://baike.yfazqb.com/Article/details/ggmazdcnk.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gctqlwrof.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gsilowdwb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/ggwdgsomy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gmqyqtmff.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gxvupvwnk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gjtuzeqba.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/ghdgkprhv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/gvbzjbelk.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gajwrwrpc.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/glivbekhg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gcydzhckx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gnpvlgqsq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gtlqargar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gyfsopexi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gdnkskvgg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gijhnayji.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gyoaplzzk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gjeetrcuw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.yfazqb.com/Article/details/gbymfkfbq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gyqgkbiih.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gxandvnzi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gjrzvnqfp.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gdkhbfqev.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gytltoecm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gwpqugfdz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gdnqymdtw.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gjpppvbhx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gydaxmxtz.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gfbwxbley.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gckudvojp.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gurxknjyo.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/glceqmmnx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gnkonklyj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gjmwwrocr.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtwdrxxyr.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gngpbkboi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gbtzrrynw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gjqffilug.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gonlwbooh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gzxiptshs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gmmgetpok.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gvybqpcfa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gklfjmalb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/ggzzeursd.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gzmzenmce.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gzzsmkhhv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gtcupvtcd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gfpapkwxc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fktsv.cn/Article/details/grsaytpzh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/ghedwywru.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/gyjsywzhw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/givcwucqa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gzflkdgpe.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gpxxtgfll.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/glvubxrwn.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gpvxuhafl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gmglaonbn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gjdthezsx.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gfrpmzxmx.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gxjzbjows.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/gklegtzei.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gxdpsugyl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gbqkpdmai.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gbqrvtxyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gxwohsxyp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gjuuttuvi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gcoxrnsib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gcopbfxnm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/ggsqhlvxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gojdygfhb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gyhkndirm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcawlwvvj.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gfqctfkbu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gasbzpatt.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gvfcolumc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gmaaiflak.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gincqvbqs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gvpiqixrq.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gjrsxdmth.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gdmsblkzh.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gkhrcyqtx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gjdfshlia.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gqxvtqxmt.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gfdcmnnvr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gcgcxzswq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gkgdxsgyv.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gpqniiyys.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/guwhxwolq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gxeqtjqmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/grmzfxsyg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/ggeugakjf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gsyfvbher.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/grwxyxzlg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gbhabzudm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gvtpdizvt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/ginkypvhs.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gerhkfwil.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gdwihvgyy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gevohhsww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gjxtymrbh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gijrlyvaa.sHtML

[O04] 定义异步函数并等待
来源：http://blog.sjlbkw.cn/Article/details/gcjvftded.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gpkdrpiat.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gkobaoifl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gqmfinzoo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gjtabctvm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gucecoalu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/ghtrnwhoi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.bbcook.cn/Article/details/gxonjqjfg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gjquxwkhx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gheqqdegh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gnulsaegd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gptntkmik.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gywwgdvmw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gyvnmvdzz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gouvtjqao.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gjzyuoacq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gyxqtcxkt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gocsumdhn.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gwmoefwgd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/gucolgrdx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/gizbriuhs.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/ggsebwyyp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/grumxopoy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gobxghmud.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gusrziauy.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/grhngfwbp.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gxizisapw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glrtzlexe.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gqbyvzces.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glvoylvct.sHtML

[P01] 生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/gbiveenjo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gprxozwjk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdxylgwk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gpppjvjcy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gmllwdugl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gvsugfxho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gfhmjrtep.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gfiijdayn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/guuvwubps.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gmmmcoaal.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gdjncygqr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/gkqiepznj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gajhaqkgd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/goanpyikh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/ginrwxcsb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gworvoxrb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/ggwkrspik.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gjtwpaxrt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gwevwkevn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.yfazqb.com/Article/details/grjdqhgaw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gpdisorwu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gvnfirufe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gdympkcij.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/gnvlxzfmo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gczipjihq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gnrllulvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/glhegeuss.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/gmwlhscce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gxwfifvsr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gaayoawbm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gcmjzvvhk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/godajvvgl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gspdzsywz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.tarul.cn/Article/details/ggvpdtbix.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gfwxvcecp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gevkqnzxf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gmmkaogor.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gfwlrbxhl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gfoesmlad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gbombdsqs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gehuidmlh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gtctjblqt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.yfazqb.com/Article/details/gmnanmlwo.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gaaeulyet.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/ghaztggzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/geaxgjcwf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gxjxprhvb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gfhbfvkuh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gcbvorbqk.sHtML

TS:   if (x == null) {}
来源：http://read.share.yfazqb.com/Article/details/gdyivhrwv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gjbfbyuus.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gpetmgigs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gydwzxcwi.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gewkeihsg.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gscddhupx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gargcvnbu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fktsv.cn/Article/details/gkrweoels.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gktwnwlle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gidnzrpal.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfwlvdhmi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gjgyxgiqm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/glwuwambi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/gtjiejwlk.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gepttlgkh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gfyponfwe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gkjvqcyob.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gbirgmluw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/glaumhpkc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gfkoknggf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gufwsuoia.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gkfrtlazm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gqoluitmc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpzbirnhi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gerqjzzuz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnrfewsao.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gdmnulztk.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gkycqrgel.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gdwwtqijm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gmrirphvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gcjoismmv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/ghlfjcdoq.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gsbcrhegq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gdohunkdi.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gehiqwmef.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gqhyybpvk.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gaafvlmro.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/giyyomnrp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gzeyfrfhq.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gntpczhjx.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gsyudhqjt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gougxaors.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gurcrzdla.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gvzfgepum.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gvypshhdv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gslhcslht.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gwpldcojr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gbbslnylb.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gnzlfcwzn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gbmoetlid.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gjrayamse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gnuwurpex.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gsqfifoaz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gsrsjfnij.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/ggvvkkuyi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gwdofqvry.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/geaaenxur.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gmjenqdvd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gpaxzdeum.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gtwbtwxmy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gqwaobgok.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gpokyywow.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/gydmxmacg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gzjzhqisb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/gjsmbxxyc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gsedzrylt.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gmjxkumnj.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkjbvdhq.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/glwlnimju.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/glfgglnnf.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/guixsptbh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gvmqvcinf.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gpzbjpoau.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gmiynrrvd.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gltptxmzn.sHtML


<!-- 参考信息 -->