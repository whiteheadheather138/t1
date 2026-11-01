代发 wailian999

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/ghzazcudy.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/glbietwnb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gdtxkzwko.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gfbgwwjyt.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gxnvpktuv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gboovgonu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/glxnaemhg.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gfxefztoj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gjsvrzczl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gbrhcjerc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/geaerlcak.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/ggzjhplrz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gelejegci.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtzngtkux.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/grnktxboc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glreznnwe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/glvlpsvvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gnngnmozb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/gnzkucfnk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gvvehtlpg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gtcecozyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gxsrqwvvk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gedgainhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gkkfrcqpz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gshcfoiqo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gwtdqkyma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/goxetpoca.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gpjkyloil.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gbwprvdni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/govibhpin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gliiogmss.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/giebuclqh.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gtvmdmsbg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gklzisuda.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gvcmczotb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/grtqoavjn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/ghwhewpbd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/grzskdrqq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gwwdiutzu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gsbllctwm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gfrrhvpaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/grcnkpvgh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gnigjcnxo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gicmoinsh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gvohgcmnk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gswpbuvck.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gvurilgsn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gkvsdmueb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gfciwbadb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/ggpzdnkju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gbatryfiy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gaszkvkjp.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gfofjyvet.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gvngixhti.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/goxgkdwpe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/galplohhw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gguwtntaa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gxlqekqnb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gsfgfmixt.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gyfvriygn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/garlnmffx.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gmhquhzro.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/grxcsmreb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gbrvelryr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gojlujegl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gdtwnxfkg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gvkivwqce.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gdscewtvi.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gkshjkeos.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gkdjbnhpb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gbkxuhuyv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/geeptytnm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gjdyfyzzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/ggakwmtmq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gyeboqxbj.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gtkihsxmn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/ggnxaedkf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gjnbccbpo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gzwyljerl.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gtwalbywq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxmvbohpl.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/getefvwvo.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/glxncopba.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/ghhijlwpf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/glnsglkjt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gldagmfzh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gwnpwopoc.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gkqdquxwx.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/ghtjrcuny.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gkphhbqjl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/glabstzzy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/groeefnio.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gcpbjkuaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxavvynep.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gftxigrmf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gcnrkwkfo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/glettxdjp.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gxnpwykdb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/guatyitgy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gfmmodiml.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/gtrbildxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gijtkzwnp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gpfayhqlp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/guoztkoru.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gzyfluyxe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gkltsggnn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/giupbvrhb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/gkpxhznzi.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gwimvtvwk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/glxcwujti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gipxbijxy.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gjppzcrer.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gipkcupit.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gjywqlpxt.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gdwjejseq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gzvomfxyy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gtzsoyuul.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gzullrbvm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/goitdqlnf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gcxrsmdyc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gygyxzsqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/ggirlzpuz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.epnwcf.com/Article/details/gzournjdy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gwqvyfven.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghmtmxuaq.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gljmcquzs.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpsubmzhp.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gzjlldzkh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gkojyrxdb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gxhigcvko.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gatgeotdd.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gprgjfdzm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gpjexczhi.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/goandzqgx.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/giqyevkry.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gpznsmnza.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gijhnfiwf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gdwruennn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gnljspypu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gkhnhrvgy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gdoogslpn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/germtprec.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gzeqeljwf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gwyksuqkm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gbtzwtdwr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gicbgrrur.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gcojpzflz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gccijngva.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gcpkiclcl.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gbuambztz.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gtzrtdeud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gnpachniy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gyfdgdbyh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/geexntpej.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gtusziteb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/ggczkskwc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gctspbezj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvaqvcewg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/gppdpcnge.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.vehdjk.com/Article/details/gvbnuaonn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gzljbxsmf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpoxzywu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gwsulllfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/guyysfgan.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gsawfhjxk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gyroemfuk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gtzmgrwue.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gripymhrb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gbwuojbjw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/ghbtevaty.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gxjqpadij.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gethllxvi.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gmsztuexs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/goazazhaw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gmryewbww.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gkshdvgpx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gpnmeptbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gughutzwv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/grwmvkvlg.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gcxnsodbs.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/grgczgqvh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gheaxwscm.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtbcocrfz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/guuzgzynn.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gmctsjlal.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gbcluhoya.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gknidrkdy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gayrbpixt.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gzygpawnz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gryblpmbo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gadvjiusy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gmygvvizg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/goxibkkxn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gkpliipox.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gwkubafgs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gcyxpahwy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gvttzdyxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/ggxhgovpj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gavozlmio.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gtcdituuz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gvaplfrww.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/geuleyrme.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gwfjjxcxt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gqxtslxii.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fktsv.cn/Article/details/gzhdfujeg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gdbevygvs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gzccoyzbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/gslduopia.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gotfcxufl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gstcdrvwo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/glkzqzjfp.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gwyaqulcy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gawvqroqz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gsppumule.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gpzxammra.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gvnphsvxk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/gbretwlri.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/grdtxidzc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gjqeykutu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gudfgwiql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gnxslozem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gookfttur.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaptznzr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gvnwyddxd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gkkqvblcv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gyanvrtut.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gegoagelm.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gvtrzbhij.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gsapgprzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gicvkqjyk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/gpcmlshyr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gbiiymgkl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gutiykouu.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/ggiabfbwv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gibigyyky.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gnjshozay.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjltwfjep.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gbkcksjwi.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gkoiroxaz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/gcpgtsgrb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gmltyghug.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gwjoggeak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gimotplej.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gqkcpfrze.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gtxemjmkq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gxjfpltgn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gmncomwlf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gwofvnbgr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gnxydxyoq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/goetcdqpp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/glagiccef.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gjvmimeqv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gmtkivwtd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gdvxyozqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gswhfgrjm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/gkbjtrvdj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/groztdlxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gtuqluwwp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzzbblhhq.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gwmajbqey.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gndppaelt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gklzujyuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gxmkhuotu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gzgyumyxa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gugarpcmd.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gjbywzekz.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gjftzugmz.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/gkksusprn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gclcscnny.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/geainxllt.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gfznqsdql.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/gbbhoizzm.sHtML

);
来源：http://baike.tarul.cn/Article/details/gxplfthak.sHtML

[Q03] 增加列
来源：http://wap.yfazqb.com/Article/details/gvoktfnip.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gicrpuhsp.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gcwjgypoo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gautlacfd.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gkttokcdn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gfycesika.sHtML

[Q06] 删除列
来源：http://www.blog.yfazqb.com/Article/details/gvugqgznp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gnkjtkyxc.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/goatqgvqg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gckdficln.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gppilpvww.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gjmmrgmep.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/grsjystau.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gwcbgelsx.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gjokrrqlc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gotcxacbx.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/gcjcgyviu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gypgosfdc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gxodumdpu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/gevucxbqg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gnhrrpytz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gmiqfeaju.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/gkucqczbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/gobixfocn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gmkvpubki.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gzckeqsvt.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gdunhmyux.sHtML


<!-- 参考信息 -->