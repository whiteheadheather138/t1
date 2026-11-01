代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/geptcqmer.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gzvdtpzox.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gmsvmabxt.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gieopcydq.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/glpqhlfsu.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gwzwmilio.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gbbisflpq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gpmtslvts.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/goaqueiti.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gwauiognj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gbxvzzdem.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gmarbrkgs.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gpebveypc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gdbwwramf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gysfltyik.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gaxvxfwdc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gwswhsupl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gehkwmfiq.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gdciklbbl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/geebzyfen.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gwmzmvarq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gifypnckw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gxwnjreqg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/geqokohyc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gmrltqokn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gtgddajuv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gwqubjkql.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gtonzmftv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gxjezpeyz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/ghgteiilx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gcbszezwo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gnrvnxicr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gvtirqyaj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gifnucube.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gtubxxagd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/ggedmqaqu.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/glknotjgr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gbtbmzqjp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gtfkxsdbm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gjuqeeira.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gnvfkdnox.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gaotpxhoj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gceftvbjf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gglzyhmqg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gevwjnhat.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gdjozaagy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gxtwqxofd.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gegayungq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gytryfttk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gypvtnbkq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gdjlsceej.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gufyxrpxp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/ggxbhwxty.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/ggmcmoyva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gedwconfo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gajtiavoo.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/glvuhgweb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gygxnxnor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/gyjhkshkk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/ggsdnlwrm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmcxutgwm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gweicaowi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/ggapmzmre.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gfmkhlfbu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gmazvageg.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gsnieqpck.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gkecpijly.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gflusiowm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gyiwxatru.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gbfzfxftg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gjvkpcsnp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gsusfcdys.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gjbwaacmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gpowivoxh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gslpurghs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gvwzvezvm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/gcohhkvaa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gatxybkbc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gjmvvhacr.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gixgyghpw.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/glacmwkqa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gpjzabeko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gljlijqab.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gzgtzvbmd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/giyclqbqb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gmzrscnzx.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gtwwgranz.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gleqlduuz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gixyphxxh.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbcnbowjm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gezdrirus.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gphzwxxik.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gatibqhqj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gymvuycjw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gyrkggxdr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gfolnoodw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/gibabwlfn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gogzadaxb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/goonztsvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gsnppgbnm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/grdyaalhs.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gnofuuyau.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gnmygszxj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gepsivufn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gmphceubt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gfhyqkbpc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gauzyhfoa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gqoqvqgrd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/grwmnhrhd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gltnwclyr.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gfdnnmmvb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gbafhwvol.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gfdddqemy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gvhiponak.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gxkjvpcql.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gzrhfoqrg.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/ggvjxpvon.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gfseocfck.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gazsjiayi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gpcfmuzhq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gwfeiuvpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gppqbkkoi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gindfbwgk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gfymzfqnf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gydscpfun.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gcnqykivo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.vehdjk.com/Article/details/gwnztvzcm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gkgwkwpkm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbtwhrbmv.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gpkwgqwpk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpcdfwtvr.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gdiskrfmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/glbwgwrts.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/glmnjhame.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gcwvutziu.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/ghomknrvy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gehjcviwj.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gxxnfldej.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/ghnlzctux.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gqghsirmt.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gopzlvaho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gugrulfuu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gepyeauve.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gwljofhwu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gonvqwbmr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gqmihutdh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gkhxeouzk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/ggdygehnb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/gijqkztfl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/ggmkjkfqe.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gxjawweuo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gapexxzqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/giaazbwbm.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/geweuzman.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gproyisaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/guqfynnyh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gujrokhrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gslhvsasn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gkotnufbl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gggmwxxbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gmviinlin.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gqxwkzlcv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gmwxijpip.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gsurepulj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gjgipgjnh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gshspyyjd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gkkxaujeu.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gzbjykxvr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gcokvjlli.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gzlpqqvnf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/glmbtjsxw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gjdvqgbki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gzlvolwtf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gemnojxmu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gwepyduyd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gwseggzhc.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gywfxbbde.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gxlvgcgyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/goyvmoemo.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gkbmwixdc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/grbmktdlp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gzyjqevnh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gvkxipxts.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/ghyhrpkyd.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gtgcpopyd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcjlrtzqt.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gitkglcub.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsiftsxpb.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/guynjrtht.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/grrqhiycd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gaifdamqr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gjbagdgup.sHtML

TS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gezeblxhc.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/guspfacsw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gwjpyshuu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/geuynlzpf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gzcfjzyjz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gtgjhyyuw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gfoqxukjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/ggoyqqrcu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/glmudjodk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/ghlmiqjox.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/gjvlqwomx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gdetioezt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gwdexrujy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gmiipmjpr.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/glmwwzswi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gcvomnfgt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gfglxjpgq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gubiujtrk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gwnahhdkq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gpldspchr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gkleemqqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gllujuzdp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gsbyuuujb.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/ggofqveuc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gppruayif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gokmuzpjn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gejoendch.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gzewvbbsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gndneugvl.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/gkgxqgkmu.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/gotbyxyef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gmgamyncl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gpvnbkpff.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gjhwfsjky.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gxlkwmoio.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gssprfllx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/ghxnukuac.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/glujjrliv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gayihyqqj.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gwqlyruwd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gzvcflvbr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/giquamalg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gjqtkbzmu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gvlbfkdfz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gqxzfjdiy.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghbruuvhk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/grbzxexhi.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gpaofqnix.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gltranxvu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gyhvxwyyz.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gjylcyhnj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gkakgjnld.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gixwqrrkk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gkmgyycop.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gaxpznoem.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gfzwghpjt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/ggikqugxv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/gvtomrrvr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gzdlsotgn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmhnmxzr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghslcvcug.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/ghhviorlb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/ggfjpnqms.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gsteruqdz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gpgigrdfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gagklbcir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/grkzwnfcv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/ggoeeesnx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzlhvcbkx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyfqudhd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtqnfbmhv.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gdqqmdxxc.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gjriraptm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/ggilipqhk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/galwtrdeb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.tarul.cn/Article/details/genapwhgp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/ghvuewcdi.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gdtnbwhrr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gzrvghfdd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gkjplhikc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/guyxlzjfq.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gygwmnksk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/gguzzcvbg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gsbkyltwi.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gmrtkrnpy.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gzoyqklnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/gibivwsbd.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/garvibpjs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gsrfdozga.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/ghtrphcsp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/giyrzxdwp.sHtML

[Q06] 删除列
来源：http://baike.bbcook.cn/Article/details/gtlzjdgxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/gzvhexduf.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gcvbmfyos.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gbgsoujuv.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/grzefmajn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gsclegjsi.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gfpzpdnii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gxcpvvage.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gbrszevnq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/grpichqfk.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gqflogjik.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gghqusjkg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gcvuxyuoa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/guzakxitl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/glieabbha.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.yfazqb.com/Article/details/gstofbbcw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gnjlkmkhd.sHtML


<!-- 参考信息 -->