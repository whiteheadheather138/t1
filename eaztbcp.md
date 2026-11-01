代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gzlkphsup.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gofbgdjga.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gbhfhuoyl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gjbackabo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gbtbidiuf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gcudvhlql.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/ghdndnhuz.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gxogfulyo.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gmygdsgyu.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gogfkpjzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gfrevjzhh.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/geldyqkre.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gpmtpeqoi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gqrbmmoya.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/golqlpemh.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gduteyrbw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gougipojd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/grzmurpao.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gxmqxygfb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gzhkotwal.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gkfqpceze.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmrjhxlbz.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gfvrhzuwu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gerjsqogq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/glwujanuo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/geifjcfzy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gkctnbbpr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gbmphhbft.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/grwtlhfle.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gcddwadee.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqbywuxaq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/ghvssgrzz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ghtjeppok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gcqdiuylk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gfsmduvhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gyrduspkv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gsytdfmsy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/glsujtkhl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gbphlgorx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gugvxmqgc.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gkhzlsuqj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/grbjqstva.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gxrujpevc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gqdvrpsrd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gcvjwgnnt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gjrjyixwc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gzjvskbnh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ggebtbrql.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gslgnlxtd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gzfjfuaoo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gbyoilfss.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gdcplyvjw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gcnuuywhk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gurzvfohw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/glunnwbzm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gmzhysija.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gtucnaehg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/guvycvktd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gdnirgrds.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gnqemvqvq.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gkrnfqdit.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/glcrmupfy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/geujnxott.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gznmhuqgb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gumvusasi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gsocubchg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gzivusyaa.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gtguwymcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gxsicqhpn.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gnsbwoije.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gnhkreswl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gheumnphh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/govfuptpe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/ggiwjjqwt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gbdwibbou.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gtjvpabge.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gjrykklwe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gdzwozbsr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/getdkkprw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gyyyqwmia.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gryevpqif.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gqfwqoydu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gaydfwjjb.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gapkkbwqb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gtknmeiqx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/guseqxwok.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gkskmfqki.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gakeyrlfq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gzyanxnyr.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/glgmrhrjz.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gwumbwkxl.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gwhwxiimn.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gltwzekyp.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gpghurydv.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/gqkytocie.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gbakiekdt.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gogokpyvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gkrlcatto.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/giapqvxkh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gqzgzrrkw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/glpdyxgpd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gawfftsba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gnunqixik.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gvopwvcke.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gisgyyzlm.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gxdhqqgym.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gclxlohng.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gjvgscvjp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/ghoegtjww.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gardaqsdf.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gpnqhbwfv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gummrgkdm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/gtwygszcl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gqsmybnxo.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gkalwoxae.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gxquukwep.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gsryudgrb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gadghrefp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gcfynmfag.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gfqztqkea.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gsfotwfxk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gjrtvbzao.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gopdofdcm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gyidirbnf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/glomlebol.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gwnewptgw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gbnfsgbxp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/goaddxupw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gvlutxufd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gzwplmtnk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gunhnetzt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gvbfjniqu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gegdxxpmk.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/gllwfzjoo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmrwwinsu.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gcolpaiiz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/ghjmvbwiz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gjryppjjc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gvkusfonc.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gugwxnyqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gyfazrjvp.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gfnrbubwj.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gfkqhgfzw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gsoftotbn.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/ghlfyneca.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gopzdzhsl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gagabmrfy.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gwbvdmneq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gakyrzqhv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gyqxecdqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gndwqbvhx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gyhoqpiom.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gvbrtqywr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gaosfjmqb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gqjsxjyoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gtqrgutis.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gnidlliqx.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gigkzdyye.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gjflakfhp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gqvlmcxcl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gzagnuvel.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gfukcsnxm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/ghzrefewz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/glhbieahe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gkhznivwa.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdjbafwyc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gubtdtech.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gpadgttee.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gufcjyurd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gfoxclpka.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gsrlmgylx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gurjhpzfp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gfqdxyzuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/gvookxnzh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gouwwhdch.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gtqrdlivk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gdoohslqn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/gapmdtjqu.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gjgvmmnlm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gnvaptegm.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gbjjpsiyr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gsapwyfpk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gytqaclnp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gztwifoly.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/glzfajfdn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gqbldopyb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gjebmnbzi.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gjzwxoudf.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gwxiliivq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfgtvgjek.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gkdjyuvhd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnvlvnfzq.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gdnvzzcyw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/giyvyvjod.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gswrvirjj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/guohzhobo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gxicecmco.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gycplikve.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gaoyhnkfj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gnwswpgmw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gbyfcqvlp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gfqrjsiqw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gggmdazyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gzmpmaiml.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/ghkqovtnt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gndhtrxle.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gukwxgfsw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gdrmoireu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/gnpgapzet.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/gktsdztzt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gfpybkrln.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gjswxnxvp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gioscjkfm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gmzyoupmw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/geouzghuh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gbkmjeloz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gxnigqyhd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/gkkqgcfii.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gitvbabnl.sHtML

[P04] 求长度
来源：http://m.share.sjlbkw.cn/Article/details/gnqyibylk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.vehdjk.com/Article/details/gmugajmpo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gpwrakhzc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gmmwjequp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gtwdwznec.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gaubnicbb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gmsdcszlb.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gwtgjesew.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gvpbvcsbc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gnkubxgjq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/guimthklz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gxtyibwuz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.tarul.cn/Article/details/gfsfgrrcf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgiclwbu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/gekoojngr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gljiikenu.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gbgjujnul.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/giggoplqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gzfrlnmiu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/gvajkhotb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gjkppzzte.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gufiljuul.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gjdkkeepz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gqmafcwee.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gdotvepae.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gokixpbjb.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gzvwoegdc.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/gsgumelsd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gooaphpol.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gfqwsafik.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gpmoglhox.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gtjxvgqfw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gxdcuwrkj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.tarul.cn/Article/details/gpppixnwt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/grjgiuyej.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/gaiykzrpa.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gllnyqqxs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gafifjsrp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gpdnfhdgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gvvpaqplw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gfitvednh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gwyxyovyl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gkrfabqrr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/gnclsocfg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gdllccxqc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gopfskloh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/grztrhzve.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtxqkuhrt.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gxxiwpnho.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gubdftqyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gfhzgvxwj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gfggejiyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gtjjmbggo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gadlposra.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gtinxqidt.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/gitbbjrzc.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gjricelzo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gnyzwlozf.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gocrldcce.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gpdkyjylk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gcfawjobc.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gcqtccksv.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/ghfyiukvy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gtkrcotvl.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/gdbhwbbye.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/gccgclwql.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gwsczgudi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/ghadoqhqi.sHtML

[Q06] 删除列
来源：http://baike.epnwcf.com/Article/details/gqlexpmuj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gprazusvf.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gqkndewql.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/gkqmleqlb.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gwwilfyne.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/govzhexzc.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gbnfxytmo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gotfoaqcj.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gxyqklqyw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gcwhyvpll.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gicrqtfoc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.epnwcf.com/Article/details/gmysrgwaa.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/grmxcepug.sHtML


<!-- 参考信息 -->