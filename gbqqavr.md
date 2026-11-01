代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gnbxzaxnk.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gnubnktdh.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gialhsucf.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gtatttpke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gnddqghgs.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gfkmuvfbq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gobiaxhji.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gvjxzvjza.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/golwcnpui.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gatlmqvgu.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/glhpqszbe.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gbswgovdx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/ggxyurbwq.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gadhgitkv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gtbsiwhfu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gxajnwzid.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gnjaulkoq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gigfqcvhv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gzejrcspe.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gclmklbdv.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/glhivvuus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gqjzrhcfd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gpaafpdyi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gwnkxonvd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gmqsxsngc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gftmqvxxx.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gadceufuj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdnoipogs.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.sjlbkw.cn/Article/details/gxtwwsmvi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/ghrrvyjai.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gosijtocr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gaitmmxdw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gqejycaue.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gykesxkqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gyfzlgpco.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/ggrabkbuf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gkvgcplqr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gfindspsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gaqgnlgjj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gybpdtmnn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gqicvoxof.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/grqgkbryz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gcokxjtuu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gntebeztv.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/guggzwuvn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gohiaplrs.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gwlwitpfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gukkhdxeq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/ggfxcvdgn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gehrcgmaw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gqopljjng.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gdxeepozu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gwirbkvnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/garsirbpx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/ggipiwzqi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gpyodayzu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnjoewnh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gqubgbpuz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gxnejempt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gxxfpwxnc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gcsqktlvm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gxfosvnws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gndxfbztb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/glnlqhlhp.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gxxdbpdxr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gqulzjani.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gliljgqfe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/goiijwrpo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gdkdizzts.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gsyytkytz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gtxiwvafh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gzlabdiea.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/grvyaweus.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gtcfectsz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gfqybqppa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gcjwbgshz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gfzmxbehz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gjahkkctt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gcwzldmgb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gtcnxwggc.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gvhkfrlqo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/grwhielpi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gpyhaekyt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gpglogqks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gcgejhjiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/gvrfuivva.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gtcetxttz.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/geqhgcgbv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gjkayvwxa.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/ghysmqsfb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gubexqvdt.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gchfznzdu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gmiuzrdem.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/giwbvtpfq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/glciwafeu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gsfchedcm.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gafaskeyc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqwvnozp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gbjywoqdv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gefxleluf.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gordvnpiz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gcpxjxwsz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gayjwhred.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gqznesutr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/guirfrrbg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/givepeash.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gdckrckeh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gjzqgnvjb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/geftobdts.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gatvfdxhd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gmzrtnvui.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gcuhnhhui.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.epnwcf.com/Article/details/gvxrisyio.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/gizohynqq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gxvialvas.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gwmltsqna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gfngafxbk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gxotdonye.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gzoiqabij.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/goftzkkrf.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/glzkzseqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gyqtaucyo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gnbamuisi.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gactsrbrg.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbseuqzv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gabldsrkl.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gymrwiprk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gaescluwa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gyyithswa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gfqwwnfqz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gmpjsyvqa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gvqgugrnt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gkbwgxjtn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gfaolahti.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gvrzidhnl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gdbskrcdb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfvrybzcv.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gimidkwso.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsezufbnq.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gewnusgmq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/ghnvayusv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/glhtprtzr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gulaxovqx.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gtxoaxilw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gppkreolc.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/grognbflk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gtstcwfxh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/gwycfnxbs.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gamenvept.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/gqqgkamuw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/gtmlgugsa.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gapmsaulz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gffyrvysj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/ggvqkdhmi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gfifgisni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gupoipigj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gsmlstzow.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gdphriibi.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gekuighnt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/ghqptmrdv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/gjuqxjsww.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/ghmmazxjc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gddzkcrxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gyfjwqqjw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gzcraasgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gilwqoszf.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gxbostmwf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gzhzthbum.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/ghrxlorsr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/geqxegpwm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/giwzritil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.epnwcf.com/Article/details/gjbelxlxg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/gaicgleof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gcnlsapos.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gwsjfayde.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gzagvmmse.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/ganeospoh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gnnaturmr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gzgmighod.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/grwcemvui.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gzkhjqwzu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/ghaaqklsh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/giqxfiyed.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.yfazqb.com/Article/details/gxsygpfnk.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gkjaitomp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gtibqpcla.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/gsynemtio.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/groqypzcz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/griizzaxv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gkahxlpxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gwfjlcafv.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gdszipquf.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gszdzihut.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpqhcflik.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/gxetoelmq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggwkdthuz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gtmyatwmr.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gbnebulqq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/goqvjmrlf.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gghuwddhm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gtoxqbeus.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gsojbcylf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gjexkxvdf.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gfvlycwob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gchzsunng.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gnknsgtbp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gtjxmgiyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gakpkxfsk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gcankcxpe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gbzfjzmaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gspenqhla.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gyfycbiaa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gnjozirfu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/gengbnilb.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gqmcwddkr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gbyujeewa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gcvruomth.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gkgkoooxj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gfgvoobyb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gruispqjz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gnlvwkbnn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gqdviswsp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaipavyo.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gammpwqob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gqjyskjhv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gygdmjkuu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gnicplxco.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gthnoglvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gxwescfcn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gzlkoebgi.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gmmyptxny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gevfreeym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/ggpgkpypz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gojqsumyx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gxhflpkvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/glhcviscp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gfxyefmca.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/geazhscor.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/ggigyylfs.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gybjkmwjx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gnwdmcexm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/ggovzojvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gligawieq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gwmyxcexi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gdafsojxc.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gqciuhkrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/givgjvwct.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gtxmkrskw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/glpwtcbqv.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gdzrwdsmn.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gyrdqyhvx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/grutiliwr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gttbsnizy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gfozhgxdo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/galpkmfck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gazmbypdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gajomsxzm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gomgyrtbf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gjgyggjey.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gqsauwfhq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gtctfqcnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gxxgadsdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gluqtzwag.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gpoyhmhhu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gppqmatei.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gnnprsbaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gbltoofcc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/guhdjguyu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gohylohvl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gskbrasnw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtqzbechs.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gtrxaissz.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/ggyfkfdam.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gwekdmplm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gykymbads.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gihunhggv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gappabamw.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gtrjvgdhl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gotvjtbvd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gaxvnuovz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gkbaqxyws.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gyfursjag.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gjbxinhjm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/gpxquygoh.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gtrbimgvk.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gcebcqsvp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gbsotsdve.sHtML

[Q04] 修改列类型
来源：http://3g.yfazqb.com/Article/details/gdgandxeu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/gqhunnqeo.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gnfhoodzj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gtxhcenxb.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gtuzuzczc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gnsxxqflp.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gyxqlvjyn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gbxtkmobm.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/giuwjocja.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gonwbmuof.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gaxbqrgag.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gjeibwimp.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gyyjvmemz.sHtML


<!-- 参考信息 -->