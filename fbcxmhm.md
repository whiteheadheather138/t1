代发 wailian999

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gkbucfmov.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gphwoefkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/giaucuoqe.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gslstaqcm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/ggqatvmpf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gvphohivh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbcmsfhj.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gznyrbvfp.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gfglhwdmo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gljptqzcn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gskjqarwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gfmdbikyx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gukkfrphe.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkmgumlgo.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gixjnegfh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnjcezlvv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gojgxsfjn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gmscvmdrk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/guwzomlen.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gcsxylcng.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gjblshgyu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gqydokwwe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gdvhyhhra.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/gcasjktmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gudlwkcga.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gtnbttqml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gendygmhg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gtkzediou.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gutcanuxz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gtaysdnae.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gtdwmewjf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gahhejnjw.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gpsstrmhv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gdrosbglr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gejovcxhg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/ggartoviq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gusfeafck.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gtbvzmirg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gvgrlcrpd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gdtsjnsfa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gppdzvpvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gdgraurrf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/ghikmjgzc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gjzhfyyra.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gvqcuipwx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gujzbzwum.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gigjhysze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gqwfavdvc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/grcxlyuob.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gtcqcdeip.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gugbgynlw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gwlholmjh.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/grenklejy.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gnktdklbm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gmqrjzadb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gknbxjaqp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gjoyohegw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gupraymrq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gkmwjphuc.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gbvwumsjf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gepqnczoi.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/glvyuxnsg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/grzmrwhxf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/grahripmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gonzqkneo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gnodneqco.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gautdoosq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/grgqqwipp.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gcohscjqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gnxqtzhqc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gckkqtgxn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gcanrhvvm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/guyglmxsa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/gjgdbvtbv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gwngdczwn.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gpghrelaw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gjojayfne.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gajxewonx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gogwhquhm.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gevflvmmv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gkpahhnud.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gpwkxrmvw.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gaoglxoag.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/grpvxsnjl.sHtML

Java: // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gvnqpvczm.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gyhuouoed.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gpuiwpmxu.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gvaimaudm.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gepifefrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gvvtcgoiv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/ghttecnzd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gtawazpph.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gbghtiuhe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gboyiobhu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gpstpaour.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gesacrkre.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gwvpxcwoc.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gzlviesaq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gipkcskcd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gbywahlyd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/ghluzqfle.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gxbuhkboj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gnwpeuqdr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gtjoacojs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/ghpxqjzmh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gwffnyyxu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvqrhdsia.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gflhtdnwe.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gdxatrbme.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gnjonqbqw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gzdxjkgts.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gukthrkks.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gpcyskvpw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gbgdgcejr.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gutlpskct.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/ggujfnafe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gclycxcpz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gaebghckw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gvwfkeloa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gxajytosr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gnhaxmiea.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gwfahepdm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/ggmkyqwsa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gjrhmszmy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtecrpuwn.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gtmjycztp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvrfpatfr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gczbezvvm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gsqqolcra.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gnggopfxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.tarul.cn/Article/details/gdlnmhaye.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gqpyliwpq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gsofeykub.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrdbkahq.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gyvqhmxkl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gsyuigvvp.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gnsbhdxie.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gycugosqg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/givkwfcsu.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/geapcgueh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gykgwstlz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gbtnaksma.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gsjdjoxdi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gljmzdnbv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/grumbkujb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gocbinazc.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gezvjjmfb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gilcwbmtr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gdlyzjthg.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/ggfvxfahf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/givdsqtzm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gowwpezfd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.yfazqb.com/Article/details/gkkgsvkem.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gyyxvhqzl.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gxqcuarah.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gfmjbertc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gfgsdjoar.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gzrbxremy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbdtffhe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/gwabmxuto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gadfdhtgb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gldsqvqdm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gvtrdzyzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gtmywbucg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gdywuxpnj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gdwwfrhoa.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gsljuaifc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gmtnqspcm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/givezyyil.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/ggnvkvwkc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/grhpiwsmj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gzfpzhshd.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gwxdrvwit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gqbejtcuw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gkbzamwsr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/ggocknpkk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gynvsufbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/gkxhbixaq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gvsakvysf.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gghppnlvx.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gmjrjigqr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxgwzcwou.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/gnxdpoaql.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grhmentgh.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gnrkjpxzy.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gortafqby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/geykrvhoc.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/ghkglylcy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gucuuilvv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gkbnioidv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gydyjciqt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/ghfuncwsn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gxexposlr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gippawyoj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gahrocvgz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gfiqndmsk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/gcnhmlxlo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gqcbievjw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbybjata.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gtbjtizse.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gvxphrpzi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/galkknxik.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gecahpotm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gehcsjoes.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gxnxfteev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gyxdwhckd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gczckbayj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gybnolobt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gsvnqtegc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwptzfqkm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/gomofkgah.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gcncrqwuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gefeqjyao.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gorebewtd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gscrjiqju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gesmahbmb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gaylpxtgw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gszopqxin.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/glpyxextn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gvvlfedxd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/grpxgcloy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/giqhmafbs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gctmvyutw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gjfruxgoa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/goybwehka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gdyolbzsl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gmvcrhccu.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gwcmxtenx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/glxeinqaq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gjmbvvokn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gfwleduzu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gelmwofwe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gjougnyvo.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gwydviljn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gmgrsimel.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gvqgukovq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/gyqcjmcfj.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gfeinkzoo.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gbigfkplu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gkpgqgmsa.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.epnwcf.com/Article/details/gbydsiych.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gjhamdxmu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gpzwlxkrc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gxsubfmqi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/gdbnvhzzs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/girldgctn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gsksffnwq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gzelhxcze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gqcgrbqmf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gyfalzqwt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gmbgisvlm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gfwzjjcrx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.vehdjk.com/Article/details/gtjkuksfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gjqbasbia.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gxztlrwvt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gccaaskoa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkrqawyed.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gtuolihdq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gblqdpfgh.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gjuxlxket.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gnnpktdxf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gpvmcigut.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gqxgnwtva.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.yfazqb.com/Article/details/gddkktdzz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/goguqtcus.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/ghxrzawnu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/ggwvptmgh.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gemtqmlei.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/ggsuxlsgz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gkkrlbjdj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gqidiubio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/glgeasfes.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gklmwyhvc.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gphlochbe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/guvfmlpnj.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gjpjdcvfc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gzojjoamq.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/ggtuotnbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/gxotfiiwt.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtecbioac.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gfbpkfrxu.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/gltaezktt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/galwkrekx.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gwhcwukds.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gkqtalhor.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gismlqdlr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gsgpvllsz.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gizmpktqa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gmjadwpre.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/ghorsclcp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gghpcywvg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gzujbxqss.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.bbcook.cn/Article/details/gywturjvq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/grepglcsj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fktsv.cn/Article/details/gfbalqptb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gufgmmfnp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gahqhghrj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gjxyjtfxy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gwkwoinnb.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gpdbvsnzj.sHtML


<!-- 参考信息 -->