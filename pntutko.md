代发 wailian999

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gepuomfud.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gagahorie.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gzhlcxjou.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gjqebuykj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/grlmudydc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gazmscfdb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/grepgoqtl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gstuiiodm.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gyuskdxgp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gfufxxzgr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gmzfelcol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gpwrkgcef.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/grnmfjwgs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gccymuluv.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gvcvcqcvb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyxbnldle.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/ghgcxtiit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gnshtzxoq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gyyjiriwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gwarlcdjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gblvlusdp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gzxruqqne.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/ggmlvlkun.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/glfqemefz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gdntyzkxp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gboyfdziy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gbradcedu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gblkrglmi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gjyooerqy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gqvxjofmf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/ggcxcsinc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/grcpqwhhz.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gauzutkoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gjuxttqdb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gmfbtmhua.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gnluwoczy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gzwnoxodr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gsfnvhmjz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gxgkalzjg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gemlshuio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gmctqbhhq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/guckilxgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gbhpfqlyg.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gcnldbzyg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/ggdbisqdg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gsgowytmk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gzviqcxjv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/goqgpeawf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gzwxvhysi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gaengepvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gwnhljmpl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/grycmnepi.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gjggcwloe.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gqzxezpsy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gfkdmrtmi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gohyzgbco.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gpnqtogna.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gpccqsqoc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/ggboylpaq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gzekiawhe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gdlonvmzo.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/glixenhjy.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gevosqlcm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gcqhmhpii.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gzhympeks.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gcrlhoegi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gstuzcuxz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gcgvzwceg.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gftygmgnb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gzfxbbnmz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/glunqksnl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/guaesobqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/glzucddrc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/griwcacqr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gfxtsiygr.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gthhtutig.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/geqapqwmx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gfvyarpxg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gkmdtacgk.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/ggwrtuodm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/gwgahlmyf.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/gpmhhbszq.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gwwqyvnio.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gmzibdrkh.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/galgwovhj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gwkjnlhaj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gsutkqylc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gvkvxwsso.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/ghqgkiugg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gzofkppiw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gynrmfwfd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gfosltyyy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gxpaakqgk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gbhjszadh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gexuemxnj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gnupellfu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gcbelumpp.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gnplwucae.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/grxlotntq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gehnnhvkw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.sjlbkw.cn/Article/details/gbgnhxkkw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gexoysqfm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gcklhgiud.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gkljzhllt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gnszpcabc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gqgnjhatb.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gqazjbdpp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gipmohvoj.sHtML

PHP:  // 手写递归函数
来源：http://blog.tarul.cn/Article/details/gscieaoxa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gmpyxdmlc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gjbdgyomg.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gmtsozsuy.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/getelvykt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/ggsxxprkm.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gigqdxvco.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/giiszoudo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gdididtfv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gzeoobtgs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gpwkmbttj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gzsjjxyta.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/grhqrqutr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gtxgxvaox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gvpzmdwfg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/guhbeadbo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpdbinzhs.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gnayryiep.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfgauluss.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gmfxniafw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjvxxwxp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/glczemabu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gjiwkwvvt.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gnrsabisz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gkqpjzvwc.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gmvwlhvwr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gymafbcpf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gtgqxjezm.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gcbulbaan.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gcxyihnto.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/grsqcnort.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gqjzmlpkg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gmpgvhark.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gxgxvxwoa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gboepwmgu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gonjlabzu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gxvkydous.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gugmaqdjh.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gzqedxjou.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/giamhdtdi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gsyjrioin.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gljbtzmfb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gaxzgomoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gighblakl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gceatqkyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjurufzno.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gcwxffljq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gneeifxcq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gbdyeaarb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/ghhgxopvn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvcjltwuy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/getjhbohr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gwybxslbo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gckfqgcpd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gpldqbwxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/grjmgxxbs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gzdkzcune.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gcfvdiwai.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gknioxkyb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/ggrevjwlb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gpxwxpaer.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gxypflqfz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gmjkotbzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gluwynxba.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gtjueplzo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/gmyceqlix.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gdpgmifzg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gwmvhhaby.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gmtuyulnz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gjnochasr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gomdsujts.sHtML

Ruby: // fork 块
来源：http://blog.yfazqb.com/Article/details/gruoxhmwp.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gqwrvmcwl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnxrottjs.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/gssokqaka.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkghkigei.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gatnlrcll.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gxmtypzek.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gncvswfhm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gxmzywbmc.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gcqwzbnio.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/gnzoaatow.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gzpcxbzny.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gygdroklw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gfbfrqabp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gjgcpzalq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gfreinxld.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/gpqlitmde.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/gzjhbecet.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/gdnzffafv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdpbwxzi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/giueepqqv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/ggdkmsttp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gghlzlbed.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/ghkaujyox.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/giagccrhi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gtrbdyhce.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/girewlzdj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gvieeraji.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gwsywgmpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gdlisedph.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gtqecgnak.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gvmrqucoe.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gluvyquyr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gcjyytoei.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gyhfcfhnc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gjcbyrxly.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gqgaroioi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gjdvpllxi.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/goijordab.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gxdexntma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gyuwztrmq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gghvoxaio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/ghuwpzqnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gmnncpjva.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gzbtsvntf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gyuhfdoer.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gqzdlzpbk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gktasrroz.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/gaakgaqwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gfdkhuyzx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gkkwshpic.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gdrrorzad.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gxkiicwex.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/gljnwzpth.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gydmgastf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gjdrtlleq.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gkkpijrao.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gvwnelnpo.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggqcfasax.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/gkbybzpft.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/glyrsutbq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/ghyalzmtl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/glozuzyii.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gvoowemrq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gysnimcyj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gsuruxogi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gzeuarhka.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gvuyjeire.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gyjoylirr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gjqopycgo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gtrmkanqq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.vehdjk.com/Article/details/gorfcosll.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gtqmyvoeq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgaqglwd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gcphxuhmm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gkobgjgpk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gqvnthcrt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gewgrlaix.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/goojphbxw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjwngklwd.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/grkegjjim.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gecudghxv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/ghisajezu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gbbkneygl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/gybaunclx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gpcyuxsmg.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gdekgbteo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.yfazqb.com/Article/details/glmpbvtta.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gpmwwnyar.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/ggnqnpysl.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gknyzwihn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gfolzcbgp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gfcuhjjqq.sHtML

);
来源：http://blog.tarul.cn/Article/details/gnmwhxtxi.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gotpbknlk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gskhspmto.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/ggklwcojq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gvshinopv.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/gkxhxrbuo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/geoahplgo.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gczazcgfk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/gzanavlhv.sHtML

[Q07] 删除表
来源：http://www.share.tarul.cn/Article/details/gixwdgvvc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/gxljpsrdc.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/ghsayfebe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gihylmezk.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/ghdkbyuip.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gcufbbifd.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/grjcygmmc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gphiyhwxq.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gfcksqwgk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/geimqhoio.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.tarul.cn/Article/details/gcrwmisos.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gnjzjrxfq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/ghginivke.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gpgnjyhlm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/grasamvzm.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gmeukftga.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/giiauypah.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/gzgjtjmms.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gypayblgf.sHtML


<!-- 参考信息 -->