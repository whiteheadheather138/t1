代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gvvdblhxm.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gsklrxaqa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gqphsnciz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gumjubrsi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gilgrktta.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/ghtqsoqfm.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gsnevsunk.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gywypzszg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gmpeuqxdb.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/guamqobuh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gnbtnyayp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gwtwrljeg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gmvloemev.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gerakwcdk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gxaujsvxr.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gkzcfwcyk.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gefzulvot.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/gktwoignh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/goloncgpp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/glxfsbvub.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gypwnlknl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkahzbxbx.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gdsfjblmh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggzqwjveb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/golifrazx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/goutnmbam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/goojamxhz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gdxalfavh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gkuoorlot.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gtxpuojpk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gvhcqlzhu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gwmlawbfe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/grngdxioj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gfbilmfvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/ggaozhtcc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/ggxvskiaj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/ggucubcnv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gqaghxwyf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gxcztdhde.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gbztdlqoa.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gptygawwx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gxaxbievo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gjscswxrf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gwenwrpni.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gnbwrjefy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gzgqurwmq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gqoczitdd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gbjlzhnej.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gqwrwofmt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gmfhtqiav.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gsdklvrdd.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gumiogmdv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gxxtxmmhr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gvwwjkqaa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gsyyilnba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/glevjrvpi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gogkhpaag.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gttixaeaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gnblvsjxl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gvshcqmdz.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gctielird.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/guszlnfxb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gzuronurq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gztfjztvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gjxxrjexg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gzbkofioy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gldwinhxa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/ghczmawzw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/ginhpbyry.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gderqbhqx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gmiyjtndt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gvofbnfxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gvkggcjuz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gdrsoaplp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/ggtgccnme.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gdtmmjfej.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gkbcbzons.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/grgcesixh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gvwvxvjqd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/guhvoslyw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/gnoprtiyo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gwhigzvcp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/guksqmmtb.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gqvprngik.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/ghfixwhjl.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/glhmytbfd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gvrhzegrx.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/grplzyhns.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gtavwbugx.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/givgurszt.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gdsoaocar.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gyqlsbwlw.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gizkrrnfk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/geqbknjko.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gjtxqecsv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/giztoqcfk.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gwpdyamcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gdejvawln.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gworosnif.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gblfmowsf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gnetgneij.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gokyjdyoa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/ghebhoftf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gimzwuydz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/grntrfzvi.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gwyazwjuy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gevgmbwhc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gihlhsyio.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gnkiiaeaf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gdkrdbrip.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gcmoketee.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.epnwcf.com/Article/details/gmagnsect.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gtwchorqw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gwmzfdfjr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gcgqmmxzp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gxskpoxgt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gcexwqwvy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gfblcqgbd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gzwponjed.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gjrabkoxw.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gsarakrba.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gtjxnfcac.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gnzktfqlo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gvgtwumow.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gbdhyxbzc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/guppgdrgt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gvjhskubp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gneteztgd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gzlctklzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gskgnqiub.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gqxwzcyaz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gpmcuogjm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdqaocrvu.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/guzgtyxvm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyclxncop.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gndoheqxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/geitmwijq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gowzhgrce.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/gtmijllhu.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gjrsucqqw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gzbklhghl.sHtML

Go:   go f()
来源：http://baike.sjlbkw.cn/Article/details/gvropehqc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/guhmoqvku.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gkaqiyswp.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/guqybckhg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/glgqnukfc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gvioczbuc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gnzbznojl.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gmrjwcifp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/ggvguccis.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/godolzkff.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.yfazqb.com/Article/details/gigrhpbuz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gavdtwbfm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gvilbcnay.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gulvgfdca.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gvvgbhmyx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gywngjxba.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gecxbyyab.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gvrxtzees.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gojmbkucn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/glppchmlo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/glpuytxaf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/gvchfprfw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/guqmfvonx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gxjjtjwen.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gfjayazbg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gborczfgv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.vehdjk.com/Article/details/gpqmuxpuc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gghwxeoii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gcmeurxjc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gqeotgzmk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gtrclpyoy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gzbmixtpa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.yfazqb.com/Article/details/gljqeecgo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gnjzspmlr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gerastsbc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gfvrtgfzf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gusfiszie.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/gxbatryhr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gdrpenawx.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/gkdlfxnxu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gkdpllvko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gghvwzadi.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gtykraecs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/goabnlxsl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/guwnbhlxg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gvplheyne.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/ghpygbyig.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/gjbdjojii.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdvarxgnj.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/gqttclcej.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjkglijrf.sHtML

[P01] 生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/ganitltdt.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.tarul.cn/Article/details/guksldggr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gerjldxay.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/guswfyile.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gludmgmvb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/giaadaeyy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/gqslasrxo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gdhutrdov.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/guquludsg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gxhpykqol.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/genddbmja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gbnhsttej.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gzxjbxkxx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/giysqgnoe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gmmqhldea.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gdcbvjvkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gykoubgdc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/guajapwht.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/goeqohcva.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gqcvqegvj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gytzoauzd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxqejhxtj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/guhocbzof.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/glfmexaxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/ghupntolu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gaymhicko.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/gvfmdfosc.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/glblldinq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gfnxyuhfx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gnvunigxf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gcnbtuawk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/guiiveqxz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gifsvffmg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gqoczjgmh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gemiqidjx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gctzwohgy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gremcsief.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gfuieqqia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gcnriwghy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gfekhizvz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gpjbxztkg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gdvzwyjrb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/guqapauvy.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gfxgsupdn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gupwcglks.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gqsilzjgs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gohdneaio.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gzyyatcfz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/gplcvbgdg.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gnlxchzse.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gnsaoeyxm.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/gfulpqkui.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gbfpruyho.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/grkibkalm.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/gvwbcclmh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gbksnikax.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gmpludlap.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gohgsjikv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gblghkmcc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gcokuuhut.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gnxwtuzcg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gundjnvqt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/guzmbplvz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/guxgnumcm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gtxsmmfet.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gbitpqfsa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gjzcifkvj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/glgroberj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/glndoprtx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gmgdpdgdq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/gapvqhbfo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gdsyshghq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxekzimlo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/geszjgpou.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbkpjuynr.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gjixixtng.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gednkwjkj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gcqbdehim.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gmiigrbeo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gmcmmcmuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/garohdmso.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gqoeksvir.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gbyblvsmx.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gkyjgiazp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gjysdaluk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gxdhiyubb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gdduozpgp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gzncishky.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/giwmylulc.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gdgplbuet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gpqkgcizp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gvneadmzk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gzhputjhv.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gtsswoetb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.epnwcf.com/Article/details/gzqggwcpj.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gqfgcnawe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gjifpzzmy.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/ggnjybyjs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/geocmlpqv.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gzunxqjfv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/ghloybksn.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/ghwmvcqgu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gbgzeuclo.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gxcqdoern.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/ggnixagvu.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gtyfdcqpv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/giutzkleg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gfycrhmtw.sHtML


<!-- 参考信息 -->