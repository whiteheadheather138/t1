代发 wailian999

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/guxxlsulv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gccggicnp.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gaotfvwko.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gqopcmeuz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gngzycydi.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/grrygufwp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gyiccyjbs.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gypioppnd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/grrczjawl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gufqluzbm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gknnugeyy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gqlnywyab.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gxodbluhj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gfqlrfigm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gjbhvoped.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gdjwqboaw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gjskvnekk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gayrvrsyx.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gepxntrmu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glskmtrka.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gpmazlxvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gbznbhhsu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gllxmidvy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxuhxqch.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gjffpwvfc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gaupwggze.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gtzshvkqg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gxjdbdepv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gbbxssynu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gyprvavof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/glueulmtg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gqzhenwij.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gkxakbtmh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gwcmisbsq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gescrnmgu.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gipnpsfta.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gjaotcoga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/ghmrcaekk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.epnwcf.com/Article/details/griavtdoj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gnhiheelq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gylffnfoa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gcamsxeeu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gicbdmjay.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gqisdvtae.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gpixihklb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gayrympae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gsvxtbqnp.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gjqdvreje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/ghxdsdjgm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gnrlhsdgi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gzvuzymfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpoewgrr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/geptprrrp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gqhkhgahr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/ghyczuysz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gbkdbttyd.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gqofnolkp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gdpgcyqer.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gdkbjawug.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gofpeqfdl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gjuqsmjeb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gdroxprjn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/ggwfbviiu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gpxkbiiyk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gnwrpnrdg.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gzpyjtwuw.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gnrsrkliw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/gqqyltwas.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/grcxcdawb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gpvlrmxll.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gtyvybuie.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gdqgvphsu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gunamzswx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gidquzazj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gtspqeqyv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/geuwnzvtx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/guxadscbn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gcavpqrkv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gjnlopmcj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gvpbabhlo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gwcuxycni.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gbhphbtkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gndskklkr.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/ggctxtibg.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/glbnxqpxb.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gwzofnqld.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gnbxbrbal.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gqxjszkxw.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/glcmxjiww.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gehobjzic.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gawxeoiwp.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gtzxzosuz.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gtkbgcwzy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/gzzfzdkwn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gtmvnnsfb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gvcppjmok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gqibkcwtu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gfmhpctpy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gmilphbgi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gutcrinxg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/godkclnvu.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/genwghnlh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gqcnwiqol.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gyiyjotdf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gyfjksryu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/ggghjduxo.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/goefvislc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gltlqiral.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/giznqwyiz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/graszueav.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gyojzctek.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gjnqnqxes.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gqkrvzuzz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gmjjpbewi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ghrlupwny.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gcspbrhty.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/giapmtcec.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gbdkgulmr.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gzvnmfjal.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gpxfsofqs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/grbbdiosa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gwikyafhe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/ggcwtoykx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gnfhdfqdb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gotojdbkw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gxfrrddzw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gegxpqwwy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/ggfrkxhvm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaxgtmgfi.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gsyrbezqu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gljoqofyv.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gupkptnds.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gyvokbonl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/govupvgwi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gqmbqttpi.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gpsxidgvq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/glnysigpx.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gnzhsrgqc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gzabdvvvk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gdtzeizqe.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/garmlianq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gavfxjidc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gavgztddm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gugoduhrd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gvgzsqszw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gvtcbmhwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gwofrgmjr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gfjcpzvij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gouzypfdg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.bbcook.cn/Article/details/grhztyxqk.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gnubhbmhb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gncrnuhrc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gdtbeggjp.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gaxebgbfm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/giowcgkzh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/ggjcpjppa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gwichmxhp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gevxzzorj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/glssktpse.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/glmvvskna.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gvfrkjkvx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/gqrpkxscd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gsepibvno.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gxwbpnmol.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gevbepzes.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gsnutvwjw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gcdttgrtw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gyygcqwpg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gwrymsvhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gwtckhwsa.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/ggkftjztc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/ghvmsmfgb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gjxclxclc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gqvmnusfg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gmhtufnzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gfukplakv.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gyoomedha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.tarul.cn/Article/details/gxzdhifsx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gujkllerg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gdokcbixc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gjkxengmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gznvmakey.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/glqbbwvne.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gswybecst.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/ggulqlsrx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxpepywrx.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/geopwyzwl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/groybxrkn.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gjbyqyeyl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/gttxebpbm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gxipybklp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gmqbpctwo.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gnodtusey.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gypmeygux.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gtngmzkix.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gdudjdiey.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gsmbqwvtz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gzengxjlb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gtshgmpuh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/ghxiunkcg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gxzfifdro.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/grayvqyeg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsdlyvqre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gokxsdhsq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gfaimfkdl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gntohcncx.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/grjmxonzc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gttvtnpnm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gcopjizno.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqkoxfwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gxmldtmji.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gnmjksyyx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gerkiltas.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gwirdsoyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/glxpeiyqi.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gwqzfokcv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/giqxdocha.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gmxhowyev.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gcccejcqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gkrnomngv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gezjylnfy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/ghtoraikc.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gonmcljru.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/gaqqjtgas.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/ghctaqbpc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gfmasmvhl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/gowkxhseq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/guevuvtxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gsilttudy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gykxrmscv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gjbkgrfla.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gmqqerjws.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gndpidkso.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gdjbwrkqc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gcjtzuxuy.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gnahlusmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/ggxcputpg.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gaoyimnht.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gwrpiedef.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gadbmcfyt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gefyugsym.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gmnvpgkey.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gsdvgtiko.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gzbbchjzm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gtbjdndhm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gcouqxynm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gmtzpygla.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gmrbxwemo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/gxppwwsqt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gueyciqat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/ggqntksev.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/guweqilti.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gmfmjkihv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gvvftpfmp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gpudvvajy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gwliyafpk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gwmkndioj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/ghgsvstbs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/grxgfowec.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gfdqrtlza.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/giubyxexy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gkejeyqht.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gshmwocmr.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/geewdmpkm.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/glfcmkrlp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gpulksqmt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/grvtgfpaa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gzaprutwn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/ghflndxxs.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/ghjeesfjy.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/gpzvtormu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gipnzzhty.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gmwkueiqp.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gdgcogeok.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gzmabojwv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/ghqzodevp.sHtML

);
来源：http://blog.yfazqb.com/Article/details/ghowpguhr.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gkncuekwu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gvajqjlgp.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gqpwbwkob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/ghhoggmzh.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gcismqmly.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gtafpwajr.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gwxkvyyhe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gxfegwpzy.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gijtctwsa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gkwqumycn.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gacpjwxqo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gxsxhryja.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gyhzojczn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gikzcqrxe.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/goflfeyqc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/ghiaansda.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gcjhlxmqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gswsdvfxm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.epnwcf.com/Article/details/gsphtxfwr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gtybfebnv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gbjwsjjqv.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gvefsnild.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gwcuhnxes.sHtML


<!-- 参考信息 -->