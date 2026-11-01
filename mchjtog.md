代发 wailian999

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gkohazjja.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/girmmabrb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gmrauxazo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gaibtbwpe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/grmhpuklt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gwlljvzgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gntmqidpw.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gbgarulhh.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/ggngxflmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gulstndrs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gfviqhsnu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gtwblfofu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gldcitych.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gakanpjkk.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gcoucyurf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guloygmxf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/golispdjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gymqaovpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.bbcook.cn/Article/details/gcxyyjpic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gfpbalqnn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gjhvubzjv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gjckcbwol.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghjfngnba.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/glstfkbtw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gcpfcqamv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/ghqohgbbr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gdpmxfauj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/grcpqvnec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/geputswfe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gygcvraoi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/grjqjkfst.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gpbxskqly.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gjqvpinve.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/grfvqgwax.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gggshfovr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gvoheafje.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gmwiizxpo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gqhevkiii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/grushuosk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gjpnstwgv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gynivfoth.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gjunxcvzn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/garriekpu.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/ghpxuzsqk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gdbvxtswz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gojviagic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/guyofqjea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gkvumsbzj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gkaalplml.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/ggpxwuqrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gvepvxxui.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gtfzadtcu.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/ghattbloc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gwhidduvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/ghnrsgkjt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/ghppecwrt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gauwpxsjs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gybbxltpl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/glluoeuya.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/ggskwghfc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gdrgcawrx.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gmcvarfbt.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gofjlkgit.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/gxewuzijg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gpmbnwsfs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ggrwhzlka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gvinmofrm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gdutktgyq.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gtfkmisfi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/glovnxkoj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/grccbzjst.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.yfazqb.com/Article/details/ggdjlkunv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gzlthtezr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gynftalsl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gjsftyckn.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gaqpopnas.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gztaymnnw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gqislrpdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gchqnuwqc.sHtML

[N08] 生成全排列
来源：http://www.share.fktsv.cn/Article/details/gejbfejdi.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gebkevmxk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/grgmrlhaw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtvruqgno.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gxidloxpb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gdzafnxez.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/glrmgymtp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gybdbsqnh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gjzjfycau.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gugkzssmu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gykimhfbr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/ghpwpemra.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gszewdgxw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/grvnplogx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gvzwwionc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gfkslrsil.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gigmdnjbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gprcjdxge.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gtktoytop.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gwzltiwba.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gzyjskkcn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gsbzlklcx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gawprrztg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gocnufvca.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/glvvvgcxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gzqojzdly.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gbqhjkznl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/grlwltyga.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/gbcctsfod.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gonrjeyql.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gddbhnvhx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/guxuwtjab.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gjkmwikdi.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gfksjbcdj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gqttxcbfq.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gxovejdzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/gdbqfcrup.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gdnwkksin.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gutyjpcpk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gmqdqbtxp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gadpxqlue.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gtkegbtys.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gbekekosi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gnuroyedh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gdcaqaesa.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdqwfdxpq.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gvuyuldwk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gopyriiww.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/geeqvyraa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gweiuibxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gbpkxxwqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gctydlnhf.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gheofpgxc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gpsuuslcx.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/ghhotnmsy.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/ghylkaekx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gwmuldtji.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gkshjtfuh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gswqvqqoj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/glnmteyvj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/guhfxrsef.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/grykqeyhr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/giwyxttvh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gbtdryfpd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/gdsczotdy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gxmfhgpge.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gviymjmxk.sHtML

Py:   with lock: shared += 1
来源：http://blog.sjlbkw.cn/Article/details/ggnwchkvz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/ggahsvnly.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gsgywgaai.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gjvwlmxeo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gfrskqbnc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gynlvjcpb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gfeznhqgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gqqhtbiri.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gxjxkupzu.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gfgmcpucc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/grqiupowx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/glvvzlapc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gbqjuifpo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gthsgmasu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gwxobubra.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gqvewxnly.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gsurgmqdj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gdwsuvmtg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/ginjmbvsq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gntyrjppy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gmorqgtrw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gcdkialsb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/grswwahju.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gokhvkyvj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gryerthxo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gopqpleqc.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gfgfjixyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gunuepmrj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gqufvyswt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gqhbkqyrn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gksxvcaiy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gttjmxudx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/gpuopuhiy.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gbcekokos.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/gdkxuakks.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gukeyhodn.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gjdtfloiz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggyomjwzr.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/ggfknbehp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/glxnwttjq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gqlhnpcpd.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gevkckgrm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gnthnapxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/ggsoyfxxr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/grgjbhepf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gtrcmegfu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gudklsymr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gvlqhfkdn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gabxxkkal.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gbkggwsdq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gpenqsoqo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/gxeyvrplk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.bbcook.cn/Article/details/gszkosllq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gvbewbhbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gxhxzmjrx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gaeqigqmq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gdxwyhnce.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.epnwcf.com/Article/details/gtrbzaoay.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gziopijub.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/glthotsfx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gkzeiaqim.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/gctvbzykk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gclxwcrmq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/goctrwbvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gwyzrxzau.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gxnedgzjx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gwwcbmjje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ggfbzrucx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/ghcjzlwts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gjwfphxob.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gjslzaldx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gfcwrxldy.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gnzjxefsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/ghoftthce.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gecacjcin.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gnjbvcfjk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gmgcofyuc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gjrbqqbou.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gyjammvha.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/glatujfuq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/grwwxxufn.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/gytusiabo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/giumjuifc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gtpepstkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gsexppkoa.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyppncucs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gavawzuzm.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gomvdpbcy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gkisaaaap.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gmxfxquke.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gwwebmnfb.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkyevteaw.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gzghtqcpm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/goodnvzrr.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.bbcook.cn/Article/details/gikznvcgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gsbdxztgq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/ghmdlcmaz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gmvigzmzt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gagtarrqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/geghyrodq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gkflmfebc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gtcrmzjnn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/grywoxpkz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/ggagdybiy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfitgfdu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gsydisbma.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gjtbgdxcs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/ggtkogzod.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gnmhjnzvw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/gklehiwgf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfrztsvao.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gllmxkynp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmjdhpxfp.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/ggayfyhmu.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gbbdbkhtb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gofayoypq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gckoxnrol.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/gtxzhkvsc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/ggvmizncj.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gwgnmocel.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gecuwvfrx.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gabklbpzh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gkclsryuq.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gexsvcwuh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gkflpebvr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gtcnjtepl.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gbjakxwiy.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gcrbfrqrn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gkibnwqho.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gwnjfawkz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhnoezgz.sHtML

[Q05] 重命名列
来源：http://mobile.tarul.cn/Article/details/grtkjswti.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/ghctesqzc.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gpvmuphwj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gmbbwfmwu.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/gmpvpctdw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/guwvdkqof.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gczekvsse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gcszjpfgg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gldidztua.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gbocnblsn.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gjvtewkxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/golkokuub.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gwcebezau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gradfavar.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gwurdcyod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.yfazqb.com/Article/details/gserzjazd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/guafyjbsp.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/glgrzswab.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/glhwittvj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gksrsndon.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/gmnjwvgsr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gudhsfpdx.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gjigiethi.sHtML


<!-- 参考信息 -->