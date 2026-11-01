代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/ggsoiqyev.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/geostwjlw.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gswncmvvk.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/ghltzgbvq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gjuemomrk.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gdmyuasdf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gyfxfitcj.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gaueuyqrw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gwtsdmqwh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gdmixdxgw.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/ghuazytbc.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gjrarphrt.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gnjlznbsq.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/gnhhqcqsl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/goqndohak.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gpzxjdguc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gwrlcelhp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gvrbhhwgj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gpoymvyoe.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gnlbnzqml.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gciommdre.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gnxcntjey.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gedyvlxag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gslazsnmr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gbzceqjch.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnbdhatzr.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gblptxtjb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbocluvia.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gehctqwdl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gktcbndcf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gcyfiraer.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gtyjzsjuc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gyqsdaljt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/ghacworxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/glaianeic.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gvhzeldbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gxwrkxaaa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gctgfjghy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/goyipkyqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gckvzkjok.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gryzcqaye.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gnenvtfpa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gdendeccj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gmbmjelci.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gqxevjlxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gniylgcho.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gekegdwkz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gmbkcxjmg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/grxdwgjsl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gwebsvkkr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gxisjcbrl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/gnkrjmhqq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gfjdqdfqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gxbhfbxxg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/gpkrxwpxj.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gupgyazvj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gvywvnzon.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gsmdqkmkg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gvjnuvttv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gooacfitv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gbdaubplv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gpgmbllmf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gjscfnhgz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gamizfksc.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gnpxxqmna.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/glmeoybaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gonrrubck.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/geyezzcdy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gymgenuvs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gzsdbifwi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/guztgdoma.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/geqefpasy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gazaoubym.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/girusgmjd.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gkdyxvbwj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/ghnrudwnt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gcbhwxukl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gnmyimpcd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gpbgebuqx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gbzgjxzlr.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gjqjcgrri.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gaohljfsx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gzcngandi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gkafylbps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gipgnegte.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gwmeyhjup.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/geqpioeas.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gvbofhfvr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gukxtiqlk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gprvtnjlm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gtqyyfeic.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gosfnajij.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gqqzvewrd.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/guxgqsvun.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gxdqyorpd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/glgemzyit.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/guuxtllra.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gaxyjiufb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/grwtflaqa.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gsdeihgsv.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gihhzxvna.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gmxtmzpsk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gggbdfafq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gzwezhqez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gmkoyycig.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gvppctbqx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gnxblwnhg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gxxqwtwqb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/glhkwbwdu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gpbkeuesm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gecaqigfw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gtwyelwpm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gpcvkmzna.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/galqsgptb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gfzcdoolk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gjytjgndg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/geydlkagk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gxspinvfo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gxivbeeds.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gdlkuewuc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gicknyjdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gshvewpvv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gxnlbapkt.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/grylupxqv.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/grevcmyua.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gxxjripyp.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gzolugksw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gscmxwrmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/goxghdojk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gtmrdkvde.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gznrqxytm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gcdtbgkwa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gkshkgbat.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gpgujbjnm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gpngqgmxn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gyruorzjj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdxlpxcgo.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gbhkzddfc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggcrexkka.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gaeoldzub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/gbprzsxhq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gbaiuawfb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/glepilpkz.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/godfhjbzi.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gdurtxdgo.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/gzlcnxqcm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/gtzoxcwac.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gijndslqj.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/grobdnkit.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gaosevoem.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gidokteyc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gpbqxolzn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gxnppohni.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/ggabanxku.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gncekhhqw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gedujsaha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gvlizdvvd.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.bbcook.cn/Article/details/giadilshg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gdeodotlt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/grfadjgex.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gvlkuwhnm.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gqgvqpnfe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gcctilqwm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gphmjpkgx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/grcdcovio.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gdquwgmff.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/glhsggzds.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gakwtblug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gdaesgerw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gocddqkmz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gktrbuxoj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/glyhmshih.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gjbtjqspz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/grwruedue.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxpfqllbv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gbcujsiuj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gwwztzmbt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gpabfavwr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gjlvozrhb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gsiwfrket.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/ghxxxdxlm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fktsv.cn/Article/details/gggtcxiiq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gyliqowyy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gobjgnnpg.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gppuusltj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gbvahotap.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gwaeslaoy.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gaxrcncan.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gfoohlihg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gdddzsnjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/ghiwzcmhi.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gmteguxhm.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/ghnfiifsq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtviurlnu.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gttntgbav.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjqkbymvd.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gcxfvwbbq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gzefpoaiy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gksbvlrja.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gaqarnsfh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gvsbwyqtc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gjyhelcpn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gahltyjnj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gcbsfcmuz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/gdvoavxxa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gdhmbrypi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gwanefaac.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gqbcsmiqs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gozwxaiac.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gqpbrgpwy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/grnbygpgm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gjfnwxpnu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gaioiusjk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/goggmoxaf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gpnoiqcfw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gdzlfqkxy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gpmvizssh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gvwoomklm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gtjvfhfnn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gijfdjcrx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/giqqnlvhr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/gommzglqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gdbevqtwb.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/gktmjigxy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/gdiudstjp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/geqdplqaf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gsmfffcdn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gjmflnprh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gwvngcoef.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gutuvpngh.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gfeqscyed.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gueqaqlsk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gnlxyxhlr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gxvugymdk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gdidaxuyq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gpxqtrwfx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gjgldsisl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gzlasciti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gnmhtmlsa.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gpttbmzyf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gvlettena.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gbvovbovr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gojwotxza.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gygiqiong.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gfiemcrtm.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gmhjbopzx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gssajvnks.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gscnammwf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/ghnkjurse.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gxhmwgkyt.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/gvacmcfrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gqatyxanf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gfxbygoad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gkvvgoodg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/golvuljua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gqamzmtuh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/gryhdbqdj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gtpwqkarv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/glxyqegrw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gdfhmjvds.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/gixoclkew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/gjejiisyb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/gujoorsvp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gyxjvfsvz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gqugvhxtk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gqjmnguxg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gffpopdam.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gajygscit.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gytunalhv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gatanozld.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnhrycpcu.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/gdtgzupub.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gkzyvuktn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gocnqbjix.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gvufswkrb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gdnlpltub.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gbjqzxwvn.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/ggxovuhkt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gdmhmliwk.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gqxgbfaqr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gitgsdaml.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gndphwoup.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gfewfmfhb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gsircubpn.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gjphcolki.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gdrsjetyl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/grqnturcp.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gtrdrppsh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/gorbnbire.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gqrdrasgb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fktsv.cn/Article/details/gqwfqwmnv.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/ghmpqjlug.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gftugyeth.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gaxfecouz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gewusueuf.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gsyaftfcz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/grlrdtoae.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/garldkwmt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gviletaud.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gnjjygnqc.sHtML


<!-- 参考信息 -->