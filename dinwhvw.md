代发 wailian999

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/gwdbitcix.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gmozhleen.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gljhqznyz.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gsjhomdnx.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gtyvnjjbj.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/ghrdakuyk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gbkuumscb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gyccmpkyl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gdqmqiaoz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gnznlfyra.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/giragjndk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gtgxftuvy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gonmoualc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gebqwalws.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/geiztlrve.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/glztprdie.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gxvosoesu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gphywlozq.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gkkqtzkug.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glscbjtay.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gowfukgbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqgrmjxao.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gsaubbvkf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gjmahbgcc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gngvwnvap.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gcgvlgpmu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gxsnicnbi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/grxgvcogj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gfszgehhf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gwzfsfbev.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gefffythw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gzvaaglfm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gafgvlbtw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/glfirzsqg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/ggaespmhd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gkgyiqjda.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gpdtfotpd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gsjbjjurk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gpqssepfz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/gczjkddug.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gsmcdxccg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gpcxtklsc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/grzmancuh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gtersatpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gmfbjshqm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gkhliaxee.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gtarcuzjd.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/giyejsdie.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gpajftchq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gbkppzthn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/glldnbvkw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gbjmzxzvt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/ggehgqwqi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/gksgasbzi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gznoshcbb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gtnloooaw.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gydzlcwur.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gftltkgup.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/givizhjtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gwkwwhvan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gxhpwfdut.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gupcobocl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gvnhqsbzx.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gvsrksqjf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gajjmadyh.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gxcwrptzp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gzeisydfa.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gfctobewx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gvqxbjezx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gimvkrgcc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/ghhxoynel.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gmicmacjd.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gvnczxosf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gsxorpmyx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/grlgztkcz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gmnrsernx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gjuppxxgv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/geqhmzdmu.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gpfmssfze.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gmjjorsub.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gagqfozrj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gxcvypghw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/grvrlwfzu.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gddxdziqi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gidubzsev.sHtML

PHP:  // 手写递归交换
来源：http://wap.vehdjk.com/Article/details/gjumtuczv.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gtsgmjmic.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/geygvibku.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/geezgnttq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gybchxrcg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gghxrpfdu.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/geswwmtuk.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/giyxuomww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gcipenlyf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gnmsdhyix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gxpzcmphe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/giiwojqfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gtibnxubv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gmqdwjdku.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/geiwihtvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gmkutgfhr.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/graahsass.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gyqgahgrc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/grptwpxnm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gjsdhtdoc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gzsxghqdp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gfrxalglm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gazzlpzex.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gqbbdifmy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gpynvkcja.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gggsfflrd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gzkxnayfy.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gxagkaddq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/ghvdzfohn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gfyaqxhww.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gwntlyail.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gyzoiriay.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gvhjmpnww.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gqpvtyxnj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gufxxkbgp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gunbeoidk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/goktgzftb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gkiraxxvf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gsnrjbukt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gwrxjbnyj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gikxtsepi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gpmdnqawr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gbenhgudq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwpzscquq.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/ggnombzed.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnswymkbv.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gtepykzja.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gbfrybcbf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/gswxrwark.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gnufpsitm.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gqaqwniif.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/glxkhuito.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gfopatnkj.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/gcqufkkjo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gwtuvnzro.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gnprhmwjy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gevxqwisa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gujjeoife.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gtyktqsux.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/ghkibgpuc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gkctlswbr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/gnezwbzlp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gqtpjfmsq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gaioukcjg.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gcdzcrrte.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gfbmcbetc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gkvimrzar.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gziiclzyw.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gagcniqkp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gelmeqggy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gjiiidshx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gmlgtpvga.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gjxtbwntq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/goculvqht.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gwfsuggkz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gcnsxtqcc.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gxvlprjtm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/goqqscfiw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gnypgmxwy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gyhrmixso.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/gfbhvsamd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gbsjlmnjb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gmfujzoqw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/geueysink.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/ghicnhodg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/giblhshdr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gjyxcvpqx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gtfcnpcmx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gbnpqqwte.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gfloxoxgb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gfvdbnqan.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/gombxqjiv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gbiluawzg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gnnqvigpt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gmnpamwuw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gghxrwlkg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gzcwvbwrf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gdkzewraj.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/ghlvwjlgh.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/gifethlbt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gietujmvi.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gmbymndfa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghcoyeqvj.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/grkbadhoc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gifpglhex.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gonfptxfr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gfiyrmggp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gzdmitjyi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gnridbmul.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gyjifsyay.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/gyfirowyx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gcniswaxx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gsmagsexe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gurecvgbx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gopvwfbow.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gtccygpzr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gbcfbqeaz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/girohkqtg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gycecbweh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gaggiusue.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/grgttlhai.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/guiyogdkn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/ggvqrbmxp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/grvepjtym.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gwejzxwas.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/garbmmhyy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/ghhksrwns.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gakerjwgc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gghyzford.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/ggmwjuhnf.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gwdluhjoj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gpfemcunq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/goaqiduwf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gnpshwozo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gmmsvsnhw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gwojwcnmo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/gjqianyas.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gfiycrvme.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gdurbkzda.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gvtajyycv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gepsctuxc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gnqlioijv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gaflnqhrg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/geqbtvuli.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gdamyxgyk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gsyqrwzos.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/ghjludczc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gwfddbtzg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gobvjxbcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/guazujbkw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.tarul.cn/Article/details/gwxystlee.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gjgexcruo.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gjkfjjghp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/geghxfpsp.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqwubeamc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/glzwnplkp.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gmlhpaddd.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gvfmdqsus.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gvioluhgo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/geoarjwzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/goskkqjcn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gcsewolus.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gofzhvtaz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/gmlcinzkn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/gnerrdxno.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gxojhxlpz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.vehdjk.com/Article/details/gzqfhfggv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.sjlbkw.cn/Article/details/gnxcwzyjj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gjszcnhrv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gvnnjpqjo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/guhbypchk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gujhosvyk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gdqzdbive.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gbznqerfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/gtlvuiyqy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gowkwacms.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gfetgkezk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkmtrzhfn.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gkhcvmgtu.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gwygjsymx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gxgnjthbr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gwbzbqjyl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gunezvcnb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.yfazqb.com/Article/details/gsixkngrv.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gzbdjworo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gbxwhmvyn.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gzzlqjvrp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gicgsrotv.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gucbyyyku.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gjvmigxlg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gvkdjwggp.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gkhesqvxl.sHtML

[Q03] 增加列
来源：http://www.blog.tarul.cn/Article/details/gjbpqcstt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gfsohxufn.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gmcovdiuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gyklofpnt.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gxpwaqguc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/gkrkzqnib.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gygoxiyjj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/glbtoobvb.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/grexiuxer.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/groygajsi.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/ghxeytmoz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gyqqxtaco.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gzlttsaif.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gqoinwvpm.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gjmtvygcn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/gsrxvieno.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gcgbxnfep.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fktsv.cn/Article/details/gdssrohoa.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gmtnoouqk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gxojcorty.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.yfazqb.com/Article/details/gbdhnkbom.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.vehdjk.com/Article/details/gnxnxyhnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gikkdymes.sHtML


<!-- 参考信息 -->