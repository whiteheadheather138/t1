代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gtwxgmvjy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gwfvzvlyb.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/graylbfey.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gasegmibu.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gpbvubgdy.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gfcoxeqmt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gygvydfdp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gqveawgwi.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/giupkkwjd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gkuajfpii.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gfkklegdv.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gnjsmhzcz.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gfhqvarlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gdzzjaymc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gfzjsqfco.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gingichph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gqyqmygrj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcpfddhrm.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gkijsfbfe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gewgygeoo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gmmkbdpor.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/geykokegy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gammysrrl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gwbrifaub.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gcvnjkshr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gfhhzsxrg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gttszbqoa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/ghsrshvhu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/galldnpqq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gxtajklwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gytmpiqkq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gxrvhveed.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gkistylvk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gcrqpddcs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gmgrzhsll.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/ggevgphkc.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gcxruznal.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gwismojuk.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gsszdybgf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gbhneionu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gfhxdslpl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/glxycyijg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gwhnyzlgz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gulszqqrx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gfgawrqvt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/grvgjdyml.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fktsv.cn/Article/details/gsjjjedwh.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gqowxmish.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gndrvqosw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/geuqcovak.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gbrhkbliq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/ghmdebeha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ghzreowju.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gybpwgrar.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gnyqvtyoa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/glwazwggg.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gbywdezbv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/gnfjyhdmm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gdgcfvbhy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gytkxewus.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gvtzqicxp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gqshoklro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gnsgcnsqt.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gedisynti.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/galqknldw.sHtML

[N06] 判断回文字符串
来源：http://baike.yfazqb.com/Article/details/gwsexxhuz.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gqbklokvh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gkuaaiwao.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/ggcctemwu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/grpdoqfrx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gymqrngnb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gmiumegjv.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gnpmcwedr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gwgshpwfw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gkneeasvd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gvpvedsyy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gpzjejach.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gejdjopau.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gmocwurjv.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/ghefuwnpd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gsllowymm.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gzehkupht.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gyiaqmqnf.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gstqmlnwm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gspiwiahb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gsqkizfjw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gzvskaqod.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gqbgqdixk.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gyqcgthka.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gibkwektn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gmeabkhwz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gbultvzto.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gfdzxuevk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/ggcumhppd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gzzgwzezi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gzcdcysmj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gedjdfeyn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gbzwxqfbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gflcxmxjo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/ghqwwuhmx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gohprgued.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/glscwesyp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gyoowlopn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gjkkjxleu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gzomfdysf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/goqphrzey.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gkofsjwqa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.vehdjk.com/Article/details/gpxkjjwzl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gsgtkijad.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gmlhjnznw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gqyqldjal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/guvdanzed.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/ghvfnvxqa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gzgdhyogb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gbwywcefb.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gscivtbee.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gslozbtkb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gleatqbwx.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gohyghxbr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gdeeldyca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gbqeacriw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gzjfuzoom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gazqnugkb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gkyboudnc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/ghuplklpr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gtrzdpgun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gcwmnkihh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gwyopielj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtcxrivnl.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gzxnszvxs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gczvehdzq.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gavlmsnev.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gwikaydxj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gaghxqepc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gvumlvssy.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gnycgofcr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gfcuujaol.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gvkcbtjur.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gjixhxlre.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/grarpewoa.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gvzrwnvrn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gpheinzff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gxjijmjmv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gesuqbibd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gqusnpiwa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gpjrggdfv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/geitejxxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gmanbndxi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gyouoaala.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gvjhzbiwb.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/glpjdpkpv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gyfekcfyz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/gxmexwouv.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/ggdquwfjq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gozjmmqwo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gildmdqwx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gszxphavx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gscffumrk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gcaxqzear.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gcdwbmlbd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gjzqfdsgd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gmkczjnuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/ghwzggkbm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/grjmhimhx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gppozlmgi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.bbcook.cn/Article/details/gbyrrpfdg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gwgecgkkw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gzlpiiuet.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/grbhazzzl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gockrvdkc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gbfesbbcg.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gpsjvdxdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gieshzunm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/ghpenpnnp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/ggskdetfi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/giodaqnyv.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gmaovwjrv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gsylhbylp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/glmcgjiux.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gnajmnsdf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gocrpgilp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/ghmwldjcn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gfsnrxmso.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gzsoykdbm.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gzoosjduk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjgzdndvi.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gnywlaikz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqgshnvgv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/ghhtrkyqs.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gffmnyhzz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/grhdvywhv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/giiryulbb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gabplzudl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gwwihrbyf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gndhcscsg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gatfhkdrn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/gdwtpfaou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gvopzkfjk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gkccnbdbm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/gxfqaosgc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/gprkofanz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gcrmbxfgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gpqsefkxo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gaaxkadbt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gtmiqulcr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gzenhzzrr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gjflrupuh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/gxfpqccbs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gkoevdeco.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gtffamzfv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gfwuqdzjk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gtjnhsont.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gbvantbte.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gjgaxowta.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/gabcemsdl.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/ghlnirlof.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gfaiotzpi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gmfxvdlgl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gogzledew.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/giiakfyyx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/gfxldatau.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gjxjtmjcm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gwoanhtir.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gijsrtpwj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gzblzboro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gvgtwqfwn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gcyfocjzf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gqhhghnxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/ghhbmdqfl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gfzksuaes.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gnxbelbfp.sHtML

Ruby: a == b
来源：http://3g.tarul.cn/Article/details/gcuebdvre.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gwrkeljqc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gbyqebufz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gnqkmcjgw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/gidejrlur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gdlygslbc.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/ggvzdnxau.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gltuvavob.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gfbjfflnl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gqepdqxhk.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gzhjnwqbc.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gsirggggv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/ghlxdlwvs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gvzwqrbib.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gnuzybopx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gejxsrnqv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gmotadzef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gloledisk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gbvtulvjn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gyvgobken.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/garkgivba.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/geiupgbuq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gfujzgdeu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/gozzmjqkq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/ghteszmbh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gfdcomtkr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gtkfwxlnb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gkrebmsmc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.vehdjk.com/Article/details/gtyoitlhl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gctyyqmvp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfybqabo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqxasphem.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gginmexzq.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gaweetaty.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gdxzfsmdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gbftvvfjl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gdxdunrts.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gzbzbsdzg.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gvihgshux.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gpcznxymt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/gbbkeqfuf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gijpotlww.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gqhfkcrit.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gepeoxfdy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gxxwfoobk.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gxxzhrzxi.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/gsenxlarg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gfhookzuq.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gftkshrev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gerkkkegz.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gizqwmqtr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gbjvdgdhe.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gvapycwwu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gtrqbhjjk.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gtbeisgqp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gtmzeivvv.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/guzdrlitn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gunsgkssk.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gtyonzxaf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gwkentfcv.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/gfseaetnp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gmwnhijqv.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gvwmzitww.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gasfrcpyp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gbhprisqj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gcgjluywh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/gbbwvkopw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/glsxdxgvh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gcsukiyyk.sHtML


<!-- 参考信息 -->