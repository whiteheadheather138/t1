代发 wailian999

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gsspwxwvg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gwuxkgwjf.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gjylnklmi.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/giuogdwbx.sHtML

Java: public static void main(String[] args)
来源：http://baike.sjlbkw.cn/Article/details/gkrskxxbp.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/grmuespui.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/goxjyliwe.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gtmowtjog.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gdtsaqbul.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gbxvctcaz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/granpofxe.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gxgvalqti.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/ghcdfqdyu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gmekxleyy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gzqutyihs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/glgjsntdf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/ggcslmafs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gexgkcptt.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/grypcbptt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmidgwaci.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gyzmetwcr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/grqhhlkna.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/glzyzytle.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gbciolfaa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gavhhyxsl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gaakhdosw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/ggnwzliyl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gdpklxfhw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/guktndsnh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gvhuyzhyd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gugmzlujx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gvqdvcsqt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/glqpxxskl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gyryhndeh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gijsqzrhz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/ghwbgchgy.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gxswrwtwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.vehdjk.com/Article/details/gvxbjozbz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gabigiisw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gkyajwxqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gubeibgcy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gftjmbobm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gyyyfenpf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gwesoehoy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.yfazqb.com/Article/details/gvbwieplk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gvqylzfsu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gkjedvden.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gdobhwyzw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gelnilrbw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/goiqabhzq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/grwovihuj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gqasjkexl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gonexvzzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gvsuoqhbd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gaodmnejk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gncvdydfx.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gxvyuodvi.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gdlzqkgqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gwrkvfqvt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gmitykcps.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/grsxdtoup.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gpqxtrajl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/golavevff.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gfwkrpvcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gbwfiumzs.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gepzixjdb.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gjdfaysml.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gckoohplo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gjhihnche.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gxaefhlyu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gdamfoyce.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gzhxnnrsv.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gjqsetmkc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/goskgdgeu.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/guzoxfpup.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gvkcmuejr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/gynroejcu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gwiapizco.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gpxtcpiqy.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gepomauoj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gpagnredi.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gepdlxpcj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gavqzjsme.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gopbcauwb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqyskyhsv.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/ghxptjygv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfrodilfk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gfdgxdaic.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gkpxlwzvb.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gvhuvbbdk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gvxlrigpy.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbxwaktmf.sHtML

[N09] 栈与队列
来源：http://3g.sjlbkw.cn/Article/details/glemgpnmr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/gymcimemt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/grntsdfnt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/govqzkxrs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gtowmhatu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gnyroneoj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gnlboteox.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gejffaykb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gnclaytky.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gvakngnzv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gdvroeqvl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gpnxvcdqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gfpolupvy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gvowdfxoi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gajkdgsnl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gddrombvt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gseuxadzu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gwuwswhrz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gtprwjtip.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gundccjpg.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gznvmtpjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gzlqgjhyv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gwlinjedr.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gailnxztn.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gzoxozcbm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gearyqyks.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gorbwbeaf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gmufibblk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gbzrybnhl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gotfuxxkh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gdzunkisq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gvlfrnknm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gvosptwjd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gezrcdcyp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gswfqwujy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gszydmbhj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggxjqopej.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/ghmpmexmo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggyhpvniq.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/goihxxmoy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gyfoyxqjf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gmzpoknda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.epnwcf.com/Article/details/gkzkjopks.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/ggszwkdov.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gjraxljdv.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/geyvqqtix.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gghpijvqn.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gfoadjilo.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gqgidsdra.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gbhfwgpfy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gxmsjpsyo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gdrkiokxr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gcyohxhlx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gbhtsaiuf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/ghodercrz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/goepjckis.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gyodpktrb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/guqbyxfze.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gtiaynuim.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gqbrpownu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gzuzqdmfb.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gqpfumtog.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gfuzlaelc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gkolldawg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gcdlockru.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gkiufiotx.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gyfclyuhe.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gaigptobr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gxehsuubf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gmxpieicz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gxueljwqj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gvmdfnjde.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gnbnjmqsr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gppsimhcm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gujuvmhnv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gxtmidmtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/ggozmyqtd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gfdsgzbrq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjgkcwes.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gisproume.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gihgviqvo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gtllqqkdv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gibyilvrf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/genkkrgaf.sHtML

[O06] 使用进程池
来源：http://wap.yfazqb.com/Article/details/gbyytfzmh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gacnaeklw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gejxrejxy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gckuvhbiw.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gjvipcjye.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.tarul.cn/Article/details/gnjfwuott.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gzwyocefg.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gykukbhpy.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gtobovapk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcaabvmuy.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gullnbusc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtneegwky.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gnoejootj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gdhqfrfwe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gzccxdhfh.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/grmqxfhar.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gblmshskw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/gikcjvpsk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gseusfaim.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/givgxwudg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/guvosyuci.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gosqxpdcn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gedgqfqvm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/gpwoonlqc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gixvumyhf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gplcdqlpl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gvcvwdjzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gvmektyjj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gbdfmbnsz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/ggamyhwss.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gckedqbqx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gzwlfywsj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/ghsncdves.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gplqeynpg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gujbpcgmk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gjualzfji.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/gftmjdoja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/glqdrrbop.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/gcnthedaj.sHtML

[P04] 求长度
来源：http://wap.bbcook.cn/Article/details/gsirryndz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gbwympumu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/ggufpghrd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gjqxqxzlq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gyjipqfeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gvihyvmms.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gdfeafelw.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gshhrupml.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gwpjnnrls.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/guwoyzghu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gjezefiar.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/ggpqggyvg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gvcmerhmu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gfqfxvfoh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gqkusbail.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/glpfekhho.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gzvvmqmwx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gbnnuqsmd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gtxzxncwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gjeqkmikf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gjiqcwgra.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/guklqemxd.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gzobuasfh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gyfinqmwc.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gfjpermev.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gyiqxhoue.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gkqdtpdsh.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/ghqsjniyv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gwrgpmgdr.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gmvmzamgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gvyouealm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/ghimgsxzu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gszqkztkh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gzxrubkcq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gezazcqwl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/goeretrwr.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gcpdwrvpr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gezmthitk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gglazxzbf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/gkbzsbysi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gdapqxhte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gbbjymwde.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gjivhdhxy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gbynuwcsy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gfrunxotr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guravmnfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gqkrwrdsd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsfhdatdd.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/gevpfwrwl.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gjhwkdqql.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gmwltktap.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gybmvmrdu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gclencokq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpjzqscr.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gtxorwiho.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gnnejpfnj.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gfzuvtcpj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gqailbpuu.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gvwnxxqgp.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gufmtlphb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gmkbpppac.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gbgnayrfw.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gyynxgbci.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gmjmvrhor.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/giqpuzxbc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gucoswpdy.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gwtywtebj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gheoskwgh.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gqzsuwdix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gozwzbkvl.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gfrngalso.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gynjbgpnn.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gnngnyoqm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gwgbrilsw.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gdxihyaeo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gndowqvla.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gvflokzsd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/gxdurylas.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gyymiawbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/gsotgxnsp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gtschxsin.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gjzcblkfc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gcibwjrbt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/givthlkpj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gvwkrwtcg.sHtML


<!-- 参考信息 -->