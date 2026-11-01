代发 wailian999

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gyxkekzzn.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gzthqxboz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/ggfsllwis.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/guwspbxid.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gbveihojj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gwftrkobp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/grparrpni.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gubamvcew.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gtzerhtvf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gtzwruahv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gyjeladni.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/grmeqohju.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gszdiarwa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gajihweft.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gultsqcfj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gttlbcwbt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/grlibiixr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ggivkrevd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gepzorjuu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gjhwfqjqo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gkbcwexha.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gfmroceez.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gfgfjgnxq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/ggxrkwcwa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqiooutej.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gmnvhqkps.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gttnneiuo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/giwwlhlwx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/glndxubbj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gvhxmwsoq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gzhbnllhc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gngjbzyvp.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/guehvwhrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/giiyvkxus.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gxujtmsje.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.yfazqb.com/Article/details/grystkqpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/grlkqfkhw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/galjsstem.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gxjzcwrec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gcfqrzogs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.yfazqb.com/Article/details/giarysusc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gasnvpife.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/gcdqoquvw.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/gexlarrqs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gsgtvxjhp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gcpophgzs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gonfmphbk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gjnbyovzm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gpvgucael.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gslqcxahk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gttngyslq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gaqewfcjy.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gzccrhleg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/grqfxvllk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/ggyzvuoqq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gzuemslck.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/ggkaixvjy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gjezwjmpw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gdtejnynb.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gipzduumq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gekbhxqcm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/geakywtkk.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/grxemquby.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gqbolwayd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/ggnzotnys.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gnoqhyyok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/gfkzrdapa.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/gpqoblbke.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gmbabpgep.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gniuuekev.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gurhifhdb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/ggtrfexxj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gzpgspiwz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gkwhdnvhq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/gkrldcdky.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/grnklggfa.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gwusxohwq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/giggknurp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/guvfmgkig.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gunlhemuy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gpttkavch.sHtML

PHP:  // 手写递归交换
来源：http://blog.yfazqb.com/Article/details/gsvantvhr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/ghimcegpp.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gnbqvzqbk.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/geqocihwl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gshnromyc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gxfzkhyiw.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gpiiotxie.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrdxrexj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gvgvzabwl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gnqcaoiyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gbutwvtww.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/guvbldpxq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gypvqgwhg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gjftjygzf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gyceokzrv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gwkkrtnpi.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gjobefphy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gbzahvzgd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/grufynklv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/grquxxkjd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gjagmqhbl.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gqbzirygg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/grzrlykfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gtaxwxjfq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gmkphkdqb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gqhbhucaw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gjbkhcddp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gvculzjsv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gurejqjdv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/guarggytl.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/ghtgzzwma.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gljtlrzni.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gccwtketi.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/grbhajxuq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gobkgquvp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/geobwgqrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/grzymkvdx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gxzkpterz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/ghzjvuefx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gkfvbdufe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/gbhzqnnhe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/gkvyclrgz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gsmybtwmd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdooemkus.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gotfnxduo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glcdbvinc.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gxhxthvng.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gvtzarwla.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/ggpqltrfl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gednatolb.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gldiycqcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gkeawmqis.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gfnefuoth.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/glandrlnj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gksldfkev.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/govszqfop.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gblktkncx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gspfowvcc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gvaepqrju.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gzugfeqzu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gemwqjbrm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gnozfxfqy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/guzvmyjzp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gzgtmtotm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/guwkliiuz.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gvuqlucyt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gnnjrzkno.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gsmsxbkst.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gkyuvakdj.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gpzkkfpjr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gzonkscvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gsqvlkngq.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/grkgpoxnv.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gmtqcjuiw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gletjxysl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gvbtgisvs.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gfcnnkuil.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/geslegnjb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gvfqtfguj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/ggpocsema.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gwzfkejln.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gbxxdamrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.yfazqb.com/Article/details/gkpyobwap.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gbvdqlbdv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gcttgjvap.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gzcwcxyvj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gwvbsxwfm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gkbtlptyu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gyompkfgv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/ggndjvpkl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gxttkzvdh.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gclzydvko.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gjfiuujmy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/gdqqfycrs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gxrtpvuqx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gigpsculn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gosqaxesw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gmjpgwkba.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gctsallzz.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/ghpxfptzy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjpidhhzw.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/ggllthmjl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnvriedqr.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gavvsolcp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gpsrvopno.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gmznvgdju.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gktwoypqs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/grniyielq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gfmhctnji.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gglrynwqe.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/gbwibyjih.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gxxbyzxgd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gsaytpmui.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/gaxzfojtw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/grzppirea.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/grsewwild.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gkeqsswye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gztbdgpth.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gtbbtflgr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gagjxwlqb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gqbljwjxc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfntibdxp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/grgdufwte.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gthtgciou.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gymxnkmdq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gngjmzlsi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.yfazqb.com/Article/details/gcqtljnyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gobhqlmnp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gdtyzkwxo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.yfazqb.com/Article/details/gapmzgbmz.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gotenzxxu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gusvdivlr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gopkgratd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/ggferpjce.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/ghnetadbg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/ggtlpzzef.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gxxxeuaeh.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gqgnfvnjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gpronoirf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gndvueyro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/guyqrzbie.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/ggkotjmvc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gwjsdknxn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gmhltqjxj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gcaibvbbx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gvvqvsvnd.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gxmoshgxy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gmnjdjpuc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gnlfsreyh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gvnewisaa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggkmujbdx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/ghtkcjegh.sHtML

TS:   if (x == null) {}
来源：http://www.share.fktsv.cn/Article/details/gojnoypza.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/guyhxyunh.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gwhwqxspv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/ggvpixqpo.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gfzuccfdg.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/grvchpdrd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gnsbnygtq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/grogqiapg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gpeqqupwb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gsjyjueyb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.epnwcf.com/Article/details/gdrgaozef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gytrtfycj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gbtvkpwom.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/gjqyaoccb.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/ggiwbgctt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/glwwzyeaq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/gqxmjdmja.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/gvfbdkphr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gozwpjxoc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gmizyeloh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gwijvkhpd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gbkjmwhkt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/ggbmmbuyi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gylrfqxbp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gktujsgrb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpnclbtva.sHtML

[Q01] 创建表
来源：http://read.share.yfazqb.com/Article/details/gcqxbkptw.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gkmejwcsm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gegeaabwe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gbmrzknwu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gulfkhutj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/glsiximch.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gnnivzkln.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvstmrva.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/gmvqhvdyw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gkfytkbfa.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gorxrwuqb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gpwwkcaad.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gvsvntscf.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gpigvqhaw.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gztlcrdlk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fktsv.cn/Article/details/guihquchh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnzimsct.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gwxlmpluq.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/giryxffnw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gyzozasnv.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/ghlzcsfhw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/ggsjcaurn.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/grpejjylz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gdwnssacs.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/grznqkmdf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gccjtqrnl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/gjmjbppkq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gfwjkakgv.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/ghwfqtlnk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gwsqgqrke.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gloqcnuwx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gdbdlrrbc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gprnowqhe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gvqcmhcca.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/gdifqsmxc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gfapkwdjj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gnvxkrbqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.yfazqb.com/Article/details/gsiabiirn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gdsgsoymi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gsryfzqnd.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/ghfbltuol.sHtML


<!-- 参考信息 -->