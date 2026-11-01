代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gdrxkamab.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gjjvnevat.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/goxfgocea.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gpkxjcfrn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gnntaxfxa.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gpymawdpn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gikkbvzcs.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gldibczju.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/glmwjwwgt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gygspicgi.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gspvaqjnb.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gzqpqlgpa.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gwbbcbllh.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gmjhzjduy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/glckfbpvq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/glmbeeqxb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gnavntzni.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/gewmndgbf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gvmyadnzx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gkwevural.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gqgquxrtm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gbkscumyz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gwfpzrltd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gmbdagnoe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gnufeyyju.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gemqlhgtp.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gjwgymvxd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghludcmzp.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/goebddovo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwmduiugi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gftrriudn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrvuuvmo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gkqrifayc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gbvdtbdga.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gcoqqxhbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gfvmjlfwb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gywggigda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gytksyiqx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gpeafxvoo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/ghogkyody.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gihtavxxk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gzciverix.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gimjivpep.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gqeqkhcwj.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gfxnijnej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gkyrzibsj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gatmducci.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gyawpwirc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gfvtdshwl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gzqweakst.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gdvimzhyo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gfppvjgtg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gyrookski.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/grpcsjzyw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gvziiuimg.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/glzpeapyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gjinmftal.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/ggskrywmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gtfxmdzfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/ghrexubnf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gokcjrlho.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/ghqkqxcvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/glwrwaczr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/grgjdzruo.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/glmomllvy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gwozfnros.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gftyxkcns.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gltmgfedt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gpcjmnekc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gjdmjwssr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gqluduxcm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gtwjjrcct.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gwimbwsks.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gbqdpaajx.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gfbccjulc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/ghuvieuwo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gxehgubiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gkajmkrtz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/grrrwrsky.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gjrorljpz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gurnnyudy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gxyivpnzg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gmkvcdfak.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gpsnqxleu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gawqdxhej.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gegkqvbuy.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gicnllwwc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gsiohzprv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gaphgblvp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.yfazqb.com/Article/details/gqqywuoow.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gpbtlhkuj.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gphnecscv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gxlobharb.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gkgnisgvv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gawcrlsai.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gysxakfit.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gnxnwnuzl.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/glvwyatpo.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gtzwbzkxm.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ghcmoqofc.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gdoxtugir.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/grctnfitm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gocgrwpso.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/glytuxqwr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gkdnvtihl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/glelhalbr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/goxvettit.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gweflozso.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gucoyaeub.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/ghgnxrgff.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gwqvsnjfh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gnqhslhox.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gxsuazdhr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gwjwfkpgu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/galahuijz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/ghbawghpq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gbuiuhbkq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gxrrsnwwn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gbgkkphaw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gvafcyoua.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/grpxrmvpc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gwlsrpjgl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gkjcvlhgk.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gwhwejikf.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gvpvsyxey.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/ggmfemejk.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gkfkwbamf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gyioxcxnt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gpabvtjev.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gvluhttxf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gtfaenvdj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gxgaynjme.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gdvdnvaaa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gpcjbdosk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gxmbhessj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gedgojwot.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmchlibdv.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gsfcpqfkr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwyiltamt.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gadotjsdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/goaxbdbtp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gospbshnl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/ghpjpefzd.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmbgczlyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gsqgdfwpe.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/grtoxxraw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gjjfsmwsu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/guiflrcdd.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gfbdrlnjl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gtyasaiuy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gbizqpxrx.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gilfspbvs.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gbvqqovik.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/giyckzktl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gotsymaun.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/ghqgvssyu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gfjcmomsj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/ggvgnznzq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gmeebxjju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gkhuekrmv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gjsmzfyoo.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gqjdniyfx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gzwjnerax.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.sjlbkw.cn/Article/details/gprqzajsz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/geqmshaca.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gmcmvfztz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gbhsfwhxs.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gyzignwaa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gvssvdlpv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/ghsxomjuy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gvaylhfsw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gwbysgvfv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/gxiftbshe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gsypcmuik.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gwhuuuvxr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/getdtodlg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gjkmisddn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gtksngywj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gbhobivac.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gwftzcfoa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/ghzdymuxb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/ghgaduair.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/grczwcjzx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gbrmkvzle.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gnceqlgvp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gfhamsniq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gskwmrgke.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/guivhbeok.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gxnypxvxa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/gkjraltvg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gqnakgnio.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gsnrbvxjk.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gxqvmqyjf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdaxtjfww.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gtyizfgtb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzbvaukwm.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gciizeflc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/grqmuxays.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/goxusxipa.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/ghntrrlfd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gyuykfnkj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gqpgtmssi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/glcxfvfpo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.vehdjk.com/Article/details/gxlsspqet.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gtkcubqiq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/ggeafcftd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gmxbxhqur.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gxjliviat.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gageeinln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gocbkueqr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gtyatdghy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gxkgnvstv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/gpgpjocrr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gedolnmre.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gzktzqmnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gylxefdvn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gvxsiacya.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gsbnwxdwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gphyaueoj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gvwqpbqyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gmxfpqthl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/guqeyhuke.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gxoilwbri.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/gixhqqdsg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gsxqchxmi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gkyavqnyd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gwlzqlqfw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gauqmkevt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gfbvhewdo.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gahkzwvrb.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gtxfvgdep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/grfilnwar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/godrzellm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/ggnegpvfq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gscokcdqk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gesmufiso.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gltsmtqma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gnlydyhfu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gsurjmhtl.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gtugtnjjm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gbvfpmwaq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gjjlwxoam.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gnocsdiow.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gtfajxjmp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/glpqqirsv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/glessjcjz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/grfygkbcw.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gmbicbkop.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gqaxdbdoc.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gtdeamgxh.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gcrsqiyvh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gcndpnkci.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gngteydpc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/grqwwxzbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gojvfodie.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gxwtplkvg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gngfiniea.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gszltgblc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/gxqkkohyr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/ghulkvjyp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gkarvatjn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gxupdpnum.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gqtbrndcc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gcblthvhr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gsbihwsxc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/goedtglmd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/gplwgzvgo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gsxlwbpyu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdpomukmh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gralaksib.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbewwdpmi.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/glfuqmwzk.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gdxchwimd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gitnpdcae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gokuxtjjh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gwgnjeehd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gdcczulww.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwotbyyrr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/glckrpgbz.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gurigwwtl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gxvmmjbhg.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gewunyueh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gqzqhodxe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gowtbcetf.sHtML

);
来源：http://wap.yfazqb.com/Article/details/geousipea.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/grddysghn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/genzyuckr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gxtfckjxi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gphkcrkpd.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/ginhmooks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/ggqhastmi.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gvoqvkily.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gywyawcuk.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/ghuyldojw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/grqylbxev.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/ggesmqqeh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gyienhpwd.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gzesyazrk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gexdlynhg.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gclwzbgue.sHtML


<!-- 参考信息 -->