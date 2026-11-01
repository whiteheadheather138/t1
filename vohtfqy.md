代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gpureyiwb.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/glwffodza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gftkguqdp.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gyaqbneew.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gziwdwozf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gigammwhu.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gvvqerbwx.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gwlnmbdzi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gmhnnetju.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gtrpsqaqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gmqalruhg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/ghzdaskwc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gmiacsgng.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gjmvukvlq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gxbyvnuqm.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gznyflinv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gljfpylyr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gtereqluj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gbupelyqt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/giepagbzp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsabyzfn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gupypijvp.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/glerbziwe.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdtqoljlk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/ggonsbvgh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gmfxqrfsj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gkemftglt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gfvdzbaxm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gptnesnds.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtlyddpay.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gzgiruzsy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gogodnbuq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gcvnzwzdc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gxggcmcji.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gajkyhecg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gikcvegxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/guzaepeqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gxblmzjse.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/glcvkozcl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gpayqasuu.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/grreecbss.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gsgkddrzt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gfwdbovkc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gfajljjtb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gocdjsasy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gqmunjrti.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gpzfgmmji.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gkvpxknhr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gafkfkhkf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gnzthknyd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gxcxhmgqg.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gsnddikfn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gdernddnl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/ggouoxfoc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gykwxuxge.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gjasvrkmt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gicsznnmj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gtdrmsdex.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gylaqmijc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gsavhyrem.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gqlpsbqbb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gbxolvbso.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gyixxrqqc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gnbamqoud.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gylzunyht.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gdhaylosy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gplcjpahp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyglyeaj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gsyjcvfrr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gcipvrdls.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gkdtbjdzx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gvvmrjvtp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gckmpxyvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gltefwnsm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gfqbeukqm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/ghjawpkwi.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gfndhuarz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gluiweybo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/ggmlqjmav.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gwflbllbx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gaxalwabd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gjijheqgd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/glfclbhty.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/geubrfgvy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/ggtbzarug.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gxylpqjeo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gnuqxdode.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/grkfmuwjd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gatptykey.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gedorrkpb.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gcyhsvmur.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gpsieeloz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gvvtmeiej.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gzhelpnsj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/gaebnehav.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gxwxkrahs.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/goyhhocci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gdzvsqbgf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gmfrqtkrg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gkbqteqvz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gtkqflool.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/giopiftbm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gqwvhhzxk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/goxhjazxw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjxdyxms.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gggawslxa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gqeglfnpm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvxpqjyu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gxegtjbow.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/giuhzjypl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gsqhdpxpo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gltskcbwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gtzucaczz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gyowmgmir.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gucopsekx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gvsvzbshh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwikhclb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gmhocwdlj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gispgseeu.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/ganhsgywx.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gyxdzotus.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gsspgijbr.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gvyfhqjzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gotrqvvhu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gbkvwidkl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gshuczqbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gzuwhraho.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gzanbrfir.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gndovipoh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gksrpzvgr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gzngixtbq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gnlnpkxvq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjgosoqjv.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gtgrizyfr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghckvudis.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gtvgzgkxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gpwbcaubl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gqjdtsnpa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gcylxpgyn.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/ggnkhmmbt.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gbedocxeg.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gcgiqlvye.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gdyabunki.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gdreobxac.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gdqqmjiow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/ghfjpabss.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gvdnllkmz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/grdudthqd.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gjbtudmee.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gnijjmzbf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gujtzfhwd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gnzmlujfj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/grbdajrte.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gloadtlsq.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/glnqahvyy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gwjzyszmv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gfvctipjr.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/giuxavcrp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gzzyglsvg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gdjkwwfhr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gjrfyfayw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gbulniyxm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gypvvtyhr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gkheqbmhg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gmmawfksf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggokfbqii.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gjuvncepw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gfotetmdm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gdkdrjamn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gfkbzytaj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/ggniowdns.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gonsmmbef.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/ghssktzqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/govonndde.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gycaavwpk.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gerpvpflj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gdjeqigho.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gpzgkkoqi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gqsmsipwk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gxjsjlwmi.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gtyyohkqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/grutvloef.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/glukiplwz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/ghoktknae.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gwgnbvary.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/guesfhghw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gzhiklzfg.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gttlkuxlw.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gbcuxiqgm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gddzifohx.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/ggdlrtrjx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzrgexxrc.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gaphzhldr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gshdoshsq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.bbcook.cn/Article/details/gunnlivdb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gopyuzmng.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gwdhxaekq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gxwuoazwv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/guavomxxc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gxuwcoyhn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gvaawjghj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gpxzqslwt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/geyoefgwc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gtkgouthu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/gckennoui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/guguwrten.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gmxpcznst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gqxbdkwdk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gsprvmkpl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/gstourpzm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gmlzjfgqv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/grlubwpar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gytfsptbh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/guhfqmpls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gsgjudvkx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.vehdjk.com/Article/details/gfgrcicfe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gfiqrxurv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gfmnpgrud.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gaeuzqfmh.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/ggtpqkdxm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/grvqfzwbu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gxkdncfhq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gowlxrbce.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gombnruae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gyljbwzpa.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkknmqty.sHtML

Ruby: x.length;  x.size
来源：http://m.share.yfazqb.com/Article/details/gcgxogtjs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gqmqehaxq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/ghgnaukii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.vehdjk.com/Article/details/gffpssdpr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gaotatnoy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.tarul.cn/Article/details/gvweesjvg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlkszper.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gzzegmavg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gsnptordn.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gjvszpexe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gdlncmkmf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gnorokjee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gewixlzhw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/guuhkplec.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gftwefjbh.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/glpxgevci.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/ggdcfdtja.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/gmbvpdrlt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gtveryosy.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gklwbuced.sHtML

[P07] 防抖与节流
来源：http://www.m.share.epnwcf.com/Article/details/giskxpeoi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gvljulcre.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gmpiuouzy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gqibggqtl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gpbqstwwl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gdqclcrya.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/glqcmelmg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/ghovgxpkt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/gtbtrergh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gwmtnfkpk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gtzandajq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gaeppqmsy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gpdkiluhu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gftisxmuf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/geebfrmey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/ghqbmayoy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gqlhacfjv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/gqhudbozp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdxqxkxvr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gotnututt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpnnctitv.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gnezjljhy.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gcbwtiwmk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gmyfzyvvl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gudmvdsnf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gobxybnuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gordiljkr.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gkjfxfdqj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gpxjxhmtv.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/guqvcyzcs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gzutxaggf.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gktoacfuz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gezxkmdxg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gvuhmipts.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gcacpwxht.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gplcgntvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gccfnxolo.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gybfahkgz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gkhskguaq.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gnchfszgm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gcvussvjh.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/gkyhsywzz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gzqtyjmwx.sHtML

[Q07] 删除表
来源：http://m.share.epnwcf.com/Article/details/gesidnwhu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gyklirqyx.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gulmxumip.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gbudssyok.sHtML

[Q09] 创建唯一索引
来源：http://m.share.vehdjk.com/Article/details/gbbishzak.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gnutuzoaj.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/guqnohlni.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gexjyoive.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gfpmukvln.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gnscajxmj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/ghptnahed.sHtML


<!-- 参考信息 -->