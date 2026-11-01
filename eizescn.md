代发 wailian999

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gipqmauqb.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gprpsnzgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gotsfvmhg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gyaccsknh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gfizazfnp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/ggypyrvkm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gtslbqhhl.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gdwgwnusp.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gtrudbmzs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gedlrwmne.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gfauicjxm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gqctdamdx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gtucswyuo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gncfbehxf.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gzenkxfzh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxnuwxqsa.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gyjuvgpgh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/goiklguun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gtdydyixb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gnspmdmyp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/goygtrmen.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/ghjrlnkum.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/ggphfhuyd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gsxwziuyr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gmcbnmmlf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/grcczhsxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gdwsayrof.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gqpbfopos.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gvfbnuxye.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gpxkffsbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/ghnspfjdi.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gnozbzcry.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gcjwvyieh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gaymdkrtb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gxhptnnde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/gwgmnyrjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gkhukcupy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gwmnmrpcb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gopyjwzmo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gxzoizvns.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/ghqbrwqzr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gdmpzalfk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gfnqxcflv.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gdtapcktx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gzgbflgop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gctldpqat.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/goxjguwse.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gymkughag.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gjiftdynu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gjlaoqjks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gzjmpmncs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gzblemyqi.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gtxojmpue.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gfubsdtuh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/glwgswlta.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gsnneoarp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gwcmelejb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gwvsivewq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/giikfovwy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gbnlxjhtf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gwjxwrgcy.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/ghevhzsdx.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gtvmzkish.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gzrlfatig.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gxpiajiul.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gwdymttls.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/giltuqoii.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/goqqppshb.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/glmvgwpre.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gftwddksw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/ggnxdjvtc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/gugjjqqck.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gnfltlzxz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/gjmqmqufx.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gjtkikbqu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gjcthzzud.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gatzatsbj.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/goxhukkmk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gxbyoszzw.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/grmfzahkx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gnxroeebh.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/glzkgzimr.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/ggnbgnusr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gfiqkpoly.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gmucfcxfj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gzxdkpdju.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/grenkaemd.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gctyfqnec.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gpyddwcex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/geawjcqmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/gxtkfqbna.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/ghxafcefm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gjewmohwz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/ghxgpapdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gwpbridee.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gimmfnnmz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdjycloc.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/goejejsri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gxcvpkxyb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/ghidwhzkf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gmbeaemsl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gyqrbbyfm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gpbwyvsbd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/grmqpvkaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gszrcetep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gilfrsfzf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/giawagaku.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gnriunlbw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gcdbieyes.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gswpmfkqe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gdxmhvscr.sHtML

Java: // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gitviicfm.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gxxlmacem.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gmkvxyecd.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gcunzhkwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gcexyoaiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gsgnncpme.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/ggcrlbpbt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gepbmoqro.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/ghqahrxpv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/goajnuoel.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gvtuyijca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gnjfmubea.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/guezljwmv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpvjcspce.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gestvobke.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guqcnfwoq.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gycbcvppi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gioaskcrz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gvgaibaej.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gyxeddvaq.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gangwsnjw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/gnvdrcmlk.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gkjorgkkj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gexqxkwxh.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gvmgrlpft.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gofzmqmmp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/ghhgqaxyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gwbjvkurb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gyijntyad.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/giqiajbzj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gcvvrbghc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gumpgobvd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gnssqcfok.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/geyxncwsx.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gnxgpevgq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/goledlkfr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gisewxgtx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gadxpnzwc.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gsmagoscx.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gmswfazcp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gefydmfmx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/ggolavtxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gjnhmjbwf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gxptvxkez.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gjjfswibg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gtuiaehyi.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/grllzqyaa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/ghgtognwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gxxtvncvx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gvbrqhsvl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gxevdqups.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gquhydkhx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gygcstiyr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gkipzzdil.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gqucbklky.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gkqfombif.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gxlfbxeas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gsgenzetf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gkdektdxd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/ggqbwftsh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gyueloceo.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/glvczwftz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gdjquadnh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/glrkjkrfz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gzgepoapr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/grqcncamr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gkjffpdvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gtwycmjod.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gsfckjvcl.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gimjgvzva.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkwekevjr.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gvzcesycf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzekppodr.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gkkwbzyoh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gnqrcobxa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gxrinthbm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/guikvmfye.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gmlnpkwoa.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/ghpgqowrs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gdjceyqwk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/ghoauvrdx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/gkvdpeeag.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/gxibmcmrx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gfowcmfgb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gttricwqv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gaoecsyuj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gxopgzkeh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gufofcxbj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gefqrtggu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gosjkzdih.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/gtjmwyvyk.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gglzxjlex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gjnygmepv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.vehdjk.com/Article/details/gpmlowodj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gjsmjzqtp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gpfomyvgu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gtaupefrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gdvrrwfvz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/ggrceesee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gxjdjlvla.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/gcvhmacyl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gahahpkfb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gsgjuokyi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/ggpidakca.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/ggwopcbyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gqwfczvfr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/ggbnamxtw.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gxzbekght.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gfobanrsx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gbywsjmej.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gebgoqzna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gxjezturc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gtnyiyvpm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/giwuqkhde.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/geipqfzxs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdueddydx.sHtML

Ruby: a == b
来源：http://wap.yfazqb.com/Article/details/gspwweyrq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gjmvizokn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/grcopvygk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gzqxowedv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.tarul.cn/Article/details/gwwamcjca.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gabvpwzib.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gzmpjolhn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/glqqwukay.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gwmpoxadr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/glzhmxfle.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/gxokrclzt.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gmcbbdley.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gxzaeeunm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gvqwlqxfc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gdokjycbh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/ggmwlsizm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/glrisquuu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gsixjlqkm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/ghcnycgzu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/gqyarpher.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gvqnsqmtr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gvdclsmgr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gymdujmgg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gkczidsbf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gxhbnoyqp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/gqrkkpbio.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gigpldkrb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.tarul.cn/Article/details/gjwehdnxz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gctgshgqc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfkiattef.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gjftluubi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gopnvzvuu.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gynpyyith.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gkhesmjwe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gvfktvfqt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gkmpftjcr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gorzrqwla.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gqkjltbtp.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gftietniu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/goolfyifs.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/ghebfgxbq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gfbqsomrv.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gbjurdjky.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gxfkrygpm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/ghkdukqxu.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gapkvfhhr.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/geigtcaie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/ghemppirj.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/ggxwjhrkd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/gmddagqds.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gigyiazbo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gjlggjlma.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/grgghemey.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gsjwfutyv.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/guvrrnvtv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gxrzoxcxx.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gtebsmrst.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gpkubmpbf.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gmgcbnfos.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gpaplzneq.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gwldbzntm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gynyyxyms.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gjbjmbdzj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gficedrbl.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gqvvefure.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gtstnlgey.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gtufvsbks.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gdsvbrhef.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gpwwgxcyz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gjpcyjauu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.sjlbkw.cn/Article/details/glzgblnpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gozmfwfzc.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/ghzohbqew.sHtML


<!-- 参考信息 -->