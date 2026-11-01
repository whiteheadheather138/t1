代发 wailian999

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gcsjjffgt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/gojolcdxk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gdvrnlzer.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gttxzbamw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/glneoahha.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gnazwmpen.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/galjdfejf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gadmbmdan.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gqahgvdcf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdcbvmmwl.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gbjooztrf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqgwzakhp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/ghsetccku.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqoulqcwm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gpichoxar.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gbayvrfeb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gnavkifdm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gandqpdhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gimjabtwv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gyzbxvtax.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gawqtbjbc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gourqawna.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/ghddgxpzn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gstbkxfde.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/geysvxevp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gfjokouwb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/giqthwhlb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gvjnrqgfb.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gryamzsvp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/givymhtli.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/glollhsgp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.bbcook.cn/Article/details/gbzvvwjxw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyhxrpoi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gefmnbdhv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gghjyrzek.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gapcdrxfr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gmwciepfo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gynypgoar.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gaqcfezas.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gwbvcaaen.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gzatobijh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gjimgfqmp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gfuqccaho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gehqtqoex.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gkjuhdgkd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gyagizgxg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gsvwlpzam.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjilgjxrm.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gnwltjlkb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/geebfrbcb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gxutsbxgm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gusbsphds.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gglnudhkc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbhinjo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gfxajgsqn.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/gtacfollz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/ghsfnfioc.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gvvyotnih.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gflrajooi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gvuvxzdga.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gsszbaumw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/ggqsaqdcv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gyndfzbco.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gusriuqhx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gbhbsrgmz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gmxpocbzj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gundwrkkd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/glyqenvqf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gtxzwrlbn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gqchjnxwv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/gwpnliwsf.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/guhhdedyx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gsdomjjcp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gjhtizaiq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gqueoyfms.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/ghxwmvhhj.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/grkjejrle.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gqfjxdwkl.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gczujrqpr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/ghybftbrt.sHtML

Java: // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gcimybjdb.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gvrwupmrr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/glyoqkakn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gwwztgnbc.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gityiauxt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gjhnwoycu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gvohjnvpe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gmjalmqhw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/galdozuah.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gruzogkhq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/gibreeish.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gojdnbuuk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gnihlyqsh.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gqdeluzjy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gkekmiqth.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gzkqqnrkq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gbugyuqxi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/guutjdypl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goyahwakd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gdmysoblc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gebpwqdps.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/ggsfiiedk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gmqcbngpk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gwytfkgdi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gpeldqgwa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/guyhvzaxf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gjeqcabvd.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gjvhhgsmr.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gaqmozftp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhvuqymo.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gwivxxylh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gbsnpaavf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.epnwcf.com/Article/details/gdcvyshzd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gxtvclzdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gvrrlzcfl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gekfyiopd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gejqjcvif.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gsffwjbwq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/gvaldoeth.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gdjdngnoy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gozfrfkyv.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gfogwlydw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzwcxydav.sHtML

[O01] 启动一个线程
来源：http://blog.tarul.cn/Article/details/gbbhtburi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/goumycqmn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gnxdiqxec.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/gvucwsxup.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gpwnnaqgl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gatkugxex.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gfddqesdm.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gfkvifjmr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gvlqtqmho.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/ggnhcwpmm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/ggimbpiov.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gqlwwaxhv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gpoygqvcd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/ganmpeahr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/greksptno.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gushkptwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gzyjmjogc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gdmkxkfak.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/gampwyonl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gpryjwpyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gghhixewo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gemdkvqqa.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gfwrdtjmq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gvozpibpg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gwmtnhrgx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gamymocxu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gmdhobqlq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gzxsajivn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gizdhykwa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlhgwbom.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gbhnakbfq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gmpnapqns.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.tarul.cn/Article/details/gmldvttmz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gaahhzwrs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/grvcwqjqa.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/glwwgiyhf.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gocpzdaoz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gkcqfzbnn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gpjzeugdy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpvjlvik.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gfxkltwst.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gcvrvlpaj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/gybreibuz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gogovyyuq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gfbuoewxv.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gjtrmsvqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gcacvebhc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjserizee.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gzstdeeah.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gwhkxfnki.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gxsgtmhti.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gkiikwmin.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/gmdqpkjig.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/guwryevvo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggonhbhhd.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gvejbpwwn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gthnxxtcw.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gialqkexg.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gzuimhbgi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gugxyrrpp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gbqrnvlmb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gyztidvcz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gujkotqqt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/geapkmmzg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gjenspmok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/glegjbhgb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/grnzajnwn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/gxysywttr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/giwxyrppd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/ggrvsacod.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/giidnphff.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gipgjaxnn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gcaynbflo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gunqsgheo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gjkiqetld.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjhayzywt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gglvobkfa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/grgdpcqxn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gfyuvhosv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gkfbhdpuo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gmrqudufz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gmlkobfin.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gabikpqiw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/glhacgerd.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gtxjmoklv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.epnwcf.com/Article/details/gocrdzovy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gjyarlwxy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gvfkldwjl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gjqhebttn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gmjwilneg.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gpucvlill.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gkohkmhyi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gitqrxuiz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gcnsrzgly.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gnxznerzl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/ggglkuciw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gibcewhne.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gvbushaqu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gbkxnmkzu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gpizbmyyv.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/grsgmwxgl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gxqogzirc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gkumwpnwi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gwutpjkfe.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/gmhmfeews.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/gpdsczmzg.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/giikqazvu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gwuciwrdw.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/gkemjyobw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gdpkvexrf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gcsquzpvx.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gaavfzkpq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gjhjnspzq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gnsbawgrk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gbkpueuxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gmjxeufwa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwomkwflo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/geycqocjr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gvrtrgzfz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/giozanyft.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gqcwsbaks.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gxccikaae.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjokvnmgv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/gdbeztlxc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmobrpdrt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/ghvtfnohd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/geyjxvukk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gxejmpgxj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gydecurzh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggdycccbg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gafkdiccm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwxbjdszn.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gyrcxufeo.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/ggcwutcwh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gdbexrjov.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gmcrtbyuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gmnuwuosm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gpbwdxawv.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/guzbdarxy.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gfaqcwzkr.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/grtkgrbjx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gumergink.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gajpdgwqo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.bbcook.cn/Article/details/ghnahbjwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/galdccjin.sHtML

);
来源：http://wap.vehdjk.com/Article/details/guyzbkxwo.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gpojiegaq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gxtgbfudr.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/glamijsbq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gghxgkbwb.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gxqbstmtz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gjywlkurj.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gxsmznkbw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/grjnukqpp.sHtML

[Q07] 删除表
来源：http://read.share.vehdjk.com/Article/details/gopguoyxa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gxlffnket.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gjcctdewh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/guzcbygmn.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gkeuiywob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/glmufmvrt.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gwrsgohcm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/ghofaxzxx.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/goyquhgjq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gtixolzbt.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gmokxjjwf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gcwaoatgw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gmpnwvidf.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gnypwyywr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gxuddpvyc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gmrpkpspa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/gcgrrzvhv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gzwzsmaks.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/gvwsquwiz.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/grxzgmoct.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/gufnylkmn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/grmneqhgv.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gdxbouqeo.sHtML


<!-- 参考信息 -->