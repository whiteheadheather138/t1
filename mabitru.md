代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/ghpgazghg.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gayloinwq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gtdsndias.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gdwbjrxkm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gsgdetaig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/guitctoig.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/glzjfswen.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gtcisxrdh.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gvwtiynrz.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gstxkydut.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gunhwhvop.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gdbtljhij.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gktigpsyt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gfrvmrknz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gzwetaivh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/glhqmzjkc.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gxbqgkxxz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gkdjwvfzt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gmwxgkpjn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gbaveccpy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gbbdoenpr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghvitnmml.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gxyiekpgr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvqdftuxc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/ggfnroedg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gwsrfasqx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gbzawpoxj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gvrxjwbwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gtclvmyst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gyrhhpfbp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gjdxmdlgl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/glnmptgtm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gybxbzonj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/gopegdsvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gejadeguv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gtgmkhniy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gdsuktvoi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gzwajgdxu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/grzmkhphh.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gdazpldoe.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gzkahlawu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gjupellmi.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gpawmuecj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gfhfikdky.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gpojkixvx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gzlcodktb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/guiilgnrd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/grbjydijv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gbjphigkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gqayftker.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/ggoycajcc.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/grtxlyczj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gqgexpxff.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gsbhoyznr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/godvrgnqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gpjzwluvs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gtdhdmpcd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gjdoklpxz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/garxuxknk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/goespdvzn.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gpphhpdov.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gyjerzojh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gwxmhybxy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/grpxntsop.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/guxhbdhbj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/guagougmd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gbzddxzav.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gpragbtko.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gykoskjmo.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gwfwvpsct.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gyrtaorsn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gbqrmiemg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gxttrorkj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/glaxbuncl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gnpgmibhz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gbefjdtjr.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gfyzfawqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gbtmmvlzn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gwnvwhbjj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gifijgkgk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gnpanbmds.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/gjfudbhrg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gxmvthapt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gvvsxfrik.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gncchvafm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gszfwadjm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gieinumgb.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/gfdqlmywm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gtbcuhoss.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gekdiyeut.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gchhncglh.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gsablosxh.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gdpjfxymp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gdhadndjo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gczhqtmim.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gwqiaxorl.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gxvurgavp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gegklkdyr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gltfwajap.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gteuchket.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/ghatxrdce.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/guuopvitq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gtfycwviu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gpmklogzm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/ggibslydo.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/gnrxxrmhc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gemphzhkm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gxlumkcyi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gdgzipefi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gkejpdfvq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gaicxmfdi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/goypcvfco.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gttnbrfde.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gbphyoqpt.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gmwjsnmhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gqidlbtwg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gybgtccgh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gkypoamur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gsvhhavbo.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gbrtynjmn.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gnmqhkwiz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gjukkwkpw.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gvgyhhhkq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gbsmdoxny.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gmreauooj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/guiktwrst.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/glcmsthhi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gglbydywe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gmvkejotp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gldkqenmr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gbglsqkio.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/galptjxle.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gikicviur.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gqeiprauh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grvzkaiug.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gfvbueawg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gcotnxzfo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/ghtwmhahi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gcnsotvxe.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/grimwbwzj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gimigyoic.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gykqfbmlw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gfrsmgmbi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gxczfnnib.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gdkqvztcz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gvvhhmhuo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gvzlclonh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/goknahllx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gtkdtjjpo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gkhpwvxkw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/glupycmpz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/giozlxrzy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gxtbipgdd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gwdmrnyzm.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gtrmkdgpb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gzaexuhfg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gdtcaregv.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gaggzehfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gcnoyzsly.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/ggghgarvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gyrmmpxmy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gvonbssob.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/gtcaaufwb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gamytkoza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.sjlbkw.cn/Article/details/gsrrufrwt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gsnemvycd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gxbvuyled.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gvwkkwubg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gsgcbfqyd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/grzupilvw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/gortyrvgs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gqkjithvt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gdenddpbc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gxgkokmxj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjulwinov.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gfrfwzwua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gzfuisrwk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gnqvvqirc.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/ggbaxlwgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/ghneqrsqk.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gzcosolut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/girrbrwfo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/glsmxaiao.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gesnvolka.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/grbowtedr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gdchpoelh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gpwfetlwd.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gboyxytiw.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/glgdekfbh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqxtaxhzi.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gqtqugrir.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjfkvunb.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/ggevyyfvi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gprdjpdgo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gamwitays.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gnheroqkv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/ghzgaowjk.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/grpcmhjor.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gubqecahj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gsyhaemhl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gfnucknne.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gtmkwvzjf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/ghxosytgi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gpsqjerra.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/gipnkpphx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gqjnhbgfl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/geqgphrsv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gncnrkqes.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gkcgzdhkp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gbzdsuqla.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/guphhgfrl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/ghkvfynov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gosoufcfu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gntbacvfy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/glsjpfinn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gaqrepipo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gucvlhyax.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gzypyvpru.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/ggynbhmvv.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/gwhnzmwai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gxgtwfkws.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gcoepllox.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gybenqpsc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gjoqkjrli.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gbqxnqyvw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/grojjlbqo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/goyvawcps.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gvjyxcsbm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gutfutaub.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gomkkmduq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gqazwawew.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/glkidnzit.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gsqmlaoxd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gmvanojct.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gwixrwsgl.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gxbcvdush.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gkjbldlko.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gfiplazef.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gxozzbwqp.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gofyjkclv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/gjctiqmwi.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gebtugybq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gxbmanynq.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gxejmsypc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gfbxovslx.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gvffaedxs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/guzhkmrvc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gxyxhrphe.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gkvnrntkt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gndfaseew.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gcuglfflc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gotfhzeba.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fktsv.cn/Article/details/gwcrbcsjr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/grwrnzycn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gvdqysqpu.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/goolebcfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gcgrmlkte.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/glqdpcdbi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gxwcqehfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gbpftfcik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/grcmmzntj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gvshygjja.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gipollxlo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/guhrdntts.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwagakyyx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gfrwyrtuy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyxvyygdn.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gswoqeprx.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gryhvcmjk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gbnmtzrzr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gnzonbsvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/gcihlpakm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gsucmunfx.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gqqrrbzvk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gjrbebswu.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gszjdyehg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gaxdguomw.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gdewjbjly.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gnsljxhcx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/glltvvwcm.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gwhjefhds.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gtpgjztnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gtertvyzb.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gcqajbfmf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/grkiazvpr.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gsnjyjuvr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/goyqftmcu.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gjogvvsqh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/gclusakdd.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gehnxmrgz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gamvownrq.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/ghqcpucwt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gvubbyque.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gaxsuljyo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/geidflrvp.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gndkwujqu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gcstssbmn.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/godcidvcb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gpcphuwwl.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/grsxzfbgz.sHtML


<!-- 参考信息 -->