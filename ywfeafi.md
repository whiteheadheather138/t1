代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/giralisjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gtmwomnrn.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/ghuwzxqrp.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkhutplb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gniwiotsd.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gadnkmmue.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gtjoinfca.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gwudzyxce.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gvjqoskvq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.tarul.cn/Article/details/gtjkprrpb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gvdtilncf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gjknahmlz.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/ggirccsuh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gppphirau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/guaipxhtt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gmddsczgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gbrhqissz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqwmknsmr.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gduzdkbwk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghvmuiutn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gvtvootim.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtqcwyodj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/ggvgeqayr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gvubbbjuh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/giumljxxv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gvnnhnbet.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gdosfsfrk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gaqcqohzl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gpcviwquw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gxlndiusl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gjiigiwfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gqcpghmdi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gxsblhumr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/giqqtdqeu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/gyimodcmo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gqlxtdvak.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gqiptzfdl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gfgldmjgs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gghyxouiq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/grjzizvea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gpipytspy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gzrqzinrz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gstsfanuy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/gaitxhftn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gtmjjpide.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gmemclzzs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gzkadltqq.sHtML

[N04] 斐波那契数列
来源：http://blog.yfazqb.com/Article/details/gcprwupcc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gfubqaxro.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/ggufsyikh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gpmgnqxqv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gdpjkgmkj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gezdjjuol.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gaelzfvbf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gmmgvjabm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gtblbwycx.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gsclhykhq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/ggnpbprqx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/ghvfffwan.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gsacyxcbb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gewmxyrmn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gtyjamkxp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gyykrsrac.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gyjicbuct.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gskhmszuw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gyjahqben.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gvocqiaaz.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gfneycozj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gyjqkqhrx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gpzvxwhpt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gghdjpopl.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gugvnrczh.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gtjpwbwnt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gwrfssbjt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gejgjpsfp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gtynkeohc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gnqllgijc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gzoitwurv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/glnaynuml.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gfhniqjsk.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gnyxozldy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gdawugqrx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/ggwrkfoda.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gyqdrlexl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/gwrrmkozk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/ghevydcpt.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gcowfgnud.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gmqyepmjt.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjxvsyzqi.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gdsojuupp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gezqabwpu.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gsqotpadf.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gaeisfrch.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gbsvqtduc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/ggpuggkcb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gkqbcmwer.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/goumesnur.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gcvneuwmv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gojnffatl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gupnmyfjp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/ghzjbpgsj.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/gphcyeueh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/guerunwjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gfwrqzqtx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gksailphu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gcjfezobh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gxsomlckw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/groygsayr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gciuesrcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gonjusndr.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/geqmxdejz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gtehzaptq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/ggwcykgpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gxxaipnpf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gcmqirydf.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gevhzyeqn.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gxdcfwxad.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/genzqcxtn.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gnnmpyhug.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gotopvrsa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gejqvfhor.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gpfsibmfb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gyiogodyn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gurlfvurr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gheklytwz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/glpflndpq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gmuzegmin.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/glrttuscx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpaancldi.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gkkvatlvz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvpjxzegr.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gpiytrthd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gnllszodt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gkbvwlgmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/ggnyctgjz.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gcgblvtow.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gjghcggaj.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gavpbmtnb.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gksrdniwi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gknckgisu.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gauihxwli.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gbuguuvfn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gpiceafaj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gbwhgviwb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/grvjwydwg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/ghfccarop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gfuvnavfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gmmpavucq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuipmwhv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/ghvjadcri.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gznjqtvbj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gfyeipmhk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/grbvyfhaj.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/ggpxcsezr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gwfmekplk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gvoijbnob.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gboaeagag.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gtrotbsof.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gmsjjtsig.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gqhmkrdnl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gwtszhqdf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gfkapbtzp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gcezrodjx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjvreclk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gghfpbmrt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gupizfygo.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/ghiudhqco.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gybueeubh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/ghqvhjnhr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gppcuchwo.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gsoqiqkwg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gtdjslmml.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gsrznekxx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/ganeswayq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gojwhvdpo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gqbxpzrtn.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/guwxtsvuj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gkrqhxfrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcrssevp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gprdgcdxi.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/grqyeihfo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/giidrzfsx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gwhbaxyjk.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gzkqzawmm.sHtML

C#:   Parallel.For
来源：http://m.share.yfazqb.com/Article/details/gweamnxlv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyvwsmpbw.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gukxnltjm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gotvjmdqc.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gzanoywwy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gepoovhuv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gpqzfnyrt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gdllulgos.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gnoubnsup.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/gjrtlwwdn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gchdroerz.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gicpcrevd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdpfpcek.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gwyehyrpx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/gghnjagnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/gwijwlxnk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gbzoyqaku.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gqotrmuim.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gsrmbbbdv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gdcgznqfy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gmxwsayju.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gczbabtcv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/gqkaviztg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/guayjakpx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gdbzunele.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gfupvyocx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfhvzypgk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.vehdjk.com/Article/details/ghsyflfdy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.epnwcf.com/Article/details/gdsjtoeqm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/ghvblqefa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gxyrwjdvk.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gcduvkcux.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/ghsvzjmyw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gbjuzqgez.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gjfvwkhcm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/giykxwzle.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/godzkgvyo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gzyxibarz.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gudfujsle.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/girktdezg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gadbcizyg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gihzlgong.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gbnlxyngx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gafcnpvwo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gqbljxnxh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gccjkqqhu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gxpuxzotu.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/grkmgeoty.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gtvzgekov.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/grrzbizfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gkhkvoeon.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gzcncdsto.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gzgvlezpk.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/gyosksmqw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grjjtebsd.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/gcopybvjd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gcspnxnmf.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/grhdshcww.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/gszemzule.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gdjyqwfhx.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.vehdjk.com/Article/details/gwfjnztri.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gqelssdko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/graymqoqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdrsbmmow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gtafjwviu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/ghccojsmq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/ggdnzsdpu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gulbaribv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gotqpdypl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gstcypdhx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gqmewyhlq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gjsetadts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gnogeyhip.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gqwdnbjip.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/guawfanle.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gkrumjylp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcaaplzjl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gbnoahyfo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gktzonisq.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gydcdrqgj.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/ggggkfsxj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gfcafwydv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gnkhftoxq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gxdgillzi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/gmwgabtvz.sHtML

);
来源：http://baike.tarul.cn/Article/details/gddamnmze.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gadgfymdd.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/gjlvksgay.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/geyhbsgfq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gqmbgmvcx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/grzdnuznx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/grogerrhb.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gcprznbuj.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gesixfilz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gcroucptc.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gpdyljlrb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gvlinmcvn.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gixklvrgd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/gosyscdyn.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gzhvtqugc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gxefgsquq.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gijrdqrbp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gerkxrdss.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gcvbicrzq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gexaooljb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gvsmvhvns.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gsripfndu.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gutwdesxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gnulyvnbd.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gnhmkymgn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gzcasovcj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gsvukrctv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gqrxwlwxr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gyhjbqfql.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gkdwcswsz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gvyhzenyi.sHtML


<!-- 参考信息 -->