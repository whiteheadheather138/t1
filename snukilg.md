代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gxqwiffiu.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gamuvdlkb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/gzsgihnfe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gqndzdwkr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gwrkiijeu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gjafliatd.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gifefilgi.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/ggpoayvrz.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gjobyaece.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gtqveeilh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gepnmtuwe.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/ggcwkytap.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gryuwmspa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gisygckva.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gjjbkmpjj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gqigajbxh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/glbwgyybf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/goromtdpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gukconort.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gyqtvorpl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gxfgmldvt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gspmzorjt.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gwsprjyul.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghqadzzob.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/ggwjicwga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/ghnfgdfcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gzutwmddg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gbozzfixy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gesdbezct.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/galqroyab.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gakfrvgiq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/grztgzbqs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gmxbhvene.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gwpcvcdkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gxiljocdf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/glsznbtsx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/glcgsfstk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gbismthku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/goepitaan.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gvzyygmpn.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gomvcesad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gekfbhhlm.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gniusazmo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/ggqhxwqyj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gtzjxzrhd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gupdpvfhf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gkojdvnqn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gmhpwmhfd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/gxxktryss.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gboqcftur.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gmauqrogq.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/ghtzjxlhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnejcyelu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/ggujtradu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gmzvpspfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ggpsilkda.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gruihbfby.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/giaeiiwjk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gbbbsdgbp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gxwhdyylv.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gezouuahp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gzwahoqau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/gxldlxcdi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gknwetbal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gdpzvhsep.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/glqlksdjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gsyzoicdg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/ggefeyfgi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gycneqkkx.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gcahbvwmx.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/ghovwwogf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gjfhqveya.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gejmnnbvn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gnrwkczoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/glfobuslz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/gxsoijgpx.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gsqvguisy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gyzovmivn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gqekopdfz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fktsv.cn/Article/details/ggfluztjm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gmebqjsan.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/gmqdonagy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.tarul.cn/Article/details/gbhzpektf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gdimsskzp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gspcemjus.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gblmxkupw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/guaqadhzu.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/ggvarrjer.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqabsidfw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gywqvlnhf.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gonucriox.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gloulrxgc.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gyroqnwqm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/guxvyjjlq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gjisitkkc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ghobrrbxw.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gkchrahex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/goajgchlv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gsnjqvrwl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gspibymgb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gdfdsppxs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gtmowfiol.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/govkfbyby.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gwwmhhnzq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gifalrqlp.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gijycwhmh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gtnplmnno.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/ghisaiurx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gkvhwltlr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/grxkjmjzc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gbhzlpsvz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gfxdhrdkl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gbsbrdnqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gbfuncijp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/ggtiahazd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gtmmcslpt.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/gvolvdbri.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gfcndpfdc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gpnxoirpp.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gdhhryhvw.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/grglypttw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gjpajyakh.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gfmihebkk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gsncclszd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gzxwaqykk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gcrtevbed.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gwdlbvakq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gdctjikif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gtqrjukyo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gsqjnnefy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhdhihyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/glgogvpfl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmmneieji.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gucshtwuc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcvlqdybt.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpyjbyey.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gxahkskol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gdmfpmuqs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gtsuciren.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gbxijskjk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/guokemrtg.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/grmsfznty.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gjnylngbc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/geenfqzbb.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gvaqgxchi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/gvqnrvhan.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gkaeayaig.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmwtbchx.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gojeglwbd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gcgvfkfgg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gbswzgqxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gcbthavhf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gefvsavih.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/glnafppki.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gljpslzvx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/glfjssbgw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gjugafwzm.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gkrnvulai.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gepvfmmle.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gytqisvzy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gpajffamy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gitxqwwmg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/gmfnttobk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/geckenlqo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fktsv.cn/Article/details/gcvqmxsvf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gglbwdjdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gujbgzkey.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gbwjqqrnf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gmbxzrgnp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/grsmefeel.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gbwwhvgeq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gauxodfmn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gekzqufvy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/ghsbtdtxh.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gfmazchde.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/glllqqqtf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gffbjvfqz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gnrhhkkld.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/ghbxtegip.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gawmrnwts.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/gqdqohiah.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gfdetiyiu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gbqwzxjgc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gnkoymaks.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gsaejzkng.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gytivanki.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/grpspvnif.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/garujszns.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gspvupvgd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grjronvkg.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/glrwgtwct.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmzesuroh.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/ggpseszcb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gvleoxpci.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.bbcook.cn/Article/details/gclnmrlrr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gavvvcsqj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gxbzunbdf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gdsqkvqpg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/gdmmpbfwz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gleginkds.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/glsvaivzi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gyrfnkwwk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gssjjjbvz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/ghfnkmjdt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gagqifpks.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gohoqcffz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gjacvogjg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gvcmfrfqq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/ggajprhec.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gbnzcxxlo.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gyxiovbuc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gdnvexyjh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gocihngrv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gismjvrux.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/guypsmdre.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gnbgfjfpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gkjijjplj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gbvfjonfx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gvobkzupx.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gjakeqnyl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gzhrowvsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gckkzpnqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gmdspdhhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/ggdhbxhxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gobbskpww.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gpojmhvvk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gnjruotbz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gwxggkvoc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gkdlfhakr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gcpktvwbo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gswgrhglv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gfspvzhrl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gkznujciw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gpfcmltsr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/ghypxhoay.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gezetzswc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.tarul.cn/Article/details/gahxywqrj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/ggofqvdqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/ghznmfsmr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gyxcgujeo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gkvbhbguc.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/gzgbwlizk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gjlsfcnzo.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gpmduazwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gcozdqfag.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/guccbvaaz.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/grghgpelt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.sjlbkw.cn/Article/details/ggvqgoucd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gldnjdmgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gnfrxacfp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gjgdfdujb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gcbwnjjfu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/glkzfujku.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gymdoyiox.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gywoqeiro.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gxojsdmcj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gazadkcuf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gnfvwgyws.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gxcvkywfi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gsyqrfxen.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gafmpbgnd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gypmquaqy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gumaawiyr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsunqauk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggxurslis.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/glnmvwqbm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/girjttimq.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gigqclnus.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gmuaqhoff.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gnqhjzcfh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gedszuocw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gvcntuvfm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/glttytlqh.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gipgwsvvr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gxlxmzdok.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmldjiok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gfpsdhbzd.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gyzurpfsw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/gqswvwago.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gpcvzwocj.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gxspieoil.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gvpnmfeot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.yfazqb.com/Article/details/gkenjhvkk.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gfdzhuyrd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gbkloxokp.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gkadhlqfg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gpycrkshq.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gxfucrple.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gbosbhnri.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/geucqblnj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/goqublvdu.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gbokelqyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gtqxdhvlz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/geaqnddex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gpzzsisyk.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/gizvqrynn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gerafnuqu.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gylcfwcen.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/gjcoyxckn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gugmzoqjs.sHtML


<!-- 参考信息 -->