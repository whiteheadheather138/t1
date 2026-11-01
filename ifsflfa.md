代发 wailian999

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/geufizpzr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gzysrdkfq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/ggonyaalc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/guvludqtn.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gepgbunwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gjklxmxsn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gnlccynkx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/guumaujuh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/grpafbmrn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxnuuvseb.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gymnuvbsm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqiifnvgy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gobwwkaby.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gxehhkdmb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gqfjjxiim.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gvlgpjuwm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/grnrkkuyq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gekxhshfd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/grtauyhkx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gybktdjcn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gueilxtwe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gktpetfxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gjhrhocse.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gycysjowg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gnnoczrhw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gflzlzzcs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gzrlurgeo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/glyncekfp.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gjcgzpnmy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gdluitrms.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/govciyryx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gtubxbjal.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gpswmyjje.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gpktdifuo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gxtspmhwu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gagorxcgs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gwihrvhzi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gxuzrydxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gtkkcerdi.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/grtfqllfy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gosnlejlb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gzpgdhxma.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gyhzjrbzd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gtdsuzrwr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gzwwujozd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gkthsupvk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/ggizvkhyk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gbwhugjhm.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gkpywewxq.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gpacbwcwa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gipqyesbc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gxhxsgxay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gifdikmtq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gytsejmxo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gogsrksva.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gizmodpmh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gxqkomkea.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/grvwgkhji.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gldkjmvxw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gkpfgeizy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gynzahdua.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/glkmyxqzy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gzrbtzjqe.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/groysorrq.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gsmurgpkr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gzqxhgumb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gatbmgdcl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gervjbmjn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gcwbdywtb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkrxtcek.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/gmnxxezts.sHtML

Java: // 手写 HashMap
来源：http://www.share.vehdjk.com/Article/details/gdlcvgthn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gnvwdpkzb.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gawuwjkjt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gfqwwxblv.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gdzruesxs.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/gkkweryok.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gvukadfcz.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gbmbpukup.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gyzfxmfie.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gtlvgwpon.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gundddgfo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/geyeikncy.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gvjxavugq.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/ginjxvhwa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/gqlzlhiba.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gznngknsm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/goiffyyqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gmswbhtgm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gbteeqyul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gqidsnegn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gsaofzwzd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gakelovqk.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gmolmhtff.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gkihvvmtd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/guktzgfjp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gaxpdizjv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gbdwzcaax.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gcldakhaz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gqffswmxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gjlsdjjjy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/glkancoqg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gvdtymzat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gfudakimy.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/grrjfqxfk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gzddrfuzw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gxtiipvsu.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gbvohyuru.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gwejhwfsu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gqkqlnldo.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/ghporuvmh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/guqibbdci.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gwecxvfrw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gkpcenmqu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gleyuotxg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gbccmtznc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gqopuwiyh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/ggsuzvdtq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gmrizanmr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gdvwfyrbo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzdfdsbww.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/glcpxwvmy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gidpoepyn.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gycdbxiok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gawxscxhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gkaqejuzg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gqjoedafg.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/goyqdyppl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/ggqozpuso.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gytwtpxkn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gfkmoaxqr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/guynyqmoc.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gsbuhujfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gajemzbij.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gqdtfqycj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gnzfbszbd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gumrasqvz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gknycnqva.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gfxxnqssw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gmbnaqtui.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gannfmyej.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gvgmpcvts.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gxlzlzyva.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gotlrgetz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/guqwjtvdr.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gmfzplhii.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gxiqwxkze.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gucluiiju.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gkiuphhdt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gbqwepjko.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/grylbbszp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gzyenerpj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gydvlxjpv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gsrymgbxw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gaztehoqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gyqbyipjq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gmrfbmsxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/gmizfwpid.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/ghrqnxnbj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gtgptkhjn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gxudkcenn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gzdrlcmnu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gqevzymly.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gmfegfpzw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gozevttjf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gcilsxzag.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gefzizsas.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gmocjwuux.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gmmzrbbvn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gcpyygnzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gaoxqrlai.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gefjueujw.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gvizvcuxu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gpbxpvofo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/genzvdnmf.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/glfyizuin.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/gymzusaix.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcoqllnqz.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/gvokssuli.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzjhqboue.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gghjvzzwo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fktsv.cn/Article/details/gnaluasse.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gfvavcwdy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/goouvsuke.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/girwuehch.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gsyyvqxif.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gutwrnxnp.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gbtafkfhk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gzivwdqka.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.tarul.cn/Article/details/gpmtnbfdu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/grnvdhbno.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gfdduqbpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gzwmaklfb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtyvnjyb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/ggduziwfh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gshxsmwwf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gaxlbsryd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gqbybrpze.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/giwvrnabo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gutfvjckc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gcguwuiff.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gimwsjwrt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gthsyctht.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gsralsmbp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gxikkffle.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gnkajycvv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/glkaglvur.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gqjjhplmb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gkwqjkgcc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gqlhtnaco.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/ggwgaotyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/glmraugdh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gbdyymnul.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/ggclneixi.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gbvjjdviz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gprejtmnk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gjuxpomnd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.epnwcf.com/Article/details/gswesoari.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gdwxuklvz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/geakbvfut.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/ghfnyvuza.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gkqvpvnsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gkjktmkdg.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/ggzzwqamj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gjgfdqzmq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gxodymbms.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gkbirtkpx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gnfynazwl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gywvvylhl.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqnzqzpca.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/ggxpborya.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtfktzkiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gviqlwcam.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gwezorxde.sHtML

[P07] 防抖与节流
来源：http://www.share.tarul.cn/Article/details/gfapekddu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/goamgsbuz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.bbcook.cn/Article/details/gookgwabr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gpcnazwmu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gkzfqhmkp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gkryfxccz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.bbcook.cn/Article/details/gzsymamox.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gxjfztvsq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gtzjylvgk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gqpxolnxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/gtdgjpmti.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gowthvhvg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gancqkzen.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpxxltaqb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gljbldbgu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gqjelowkr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gqonxgwog.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/gpzjsyxxj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbzugrhir.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/grtusvtdd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghdtsatcn.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgdnuytx.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gxlxcozoy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gtbgffpnk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/grpibjkeu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gmsnijeln.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gyxygiixb.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gnxeaplpp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gnwknmrjv.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/gteknatsx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/ggwspnxcw.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gvbdseojk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gqfnbateb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.tarul.cn/Article/details/gtthxsxro.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gvnovexso.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gjvbatsuu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gaasokicp.sHtML

[Q04] 修改列类型
来源：http://read.share.bbcook.cn/Article/details/gswasjsqm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gikodgoum.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gwzhaabgw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gswymqmok.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gpwveyjka.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gjdyktfvs.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gcnersbzd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gddzsfnno.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gxrrujnli.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gnejpfkac.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gnvojlwnl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gqdqooulu.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/gjbgdqsrh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gkeudzvbm.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gpykkrlcd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gselejvxu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gqkwsbeoj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/ggalnppie.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/greeusfmf.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gjomtakdr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gqtvzjxpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/gwkirdygh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gaylyxbhs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gnaqqyhkn.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gsunibmsw.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/ggssvzgfj.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gajrhctrp.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/glvgfzszt.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gdrrswegc.sHtML


<!-- 参考信息 -->