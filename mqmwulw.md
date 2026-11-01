代发 wailian999

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gvdwsznxd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gsvknctnp.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gyaiqgvbj.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/glvhrtkeo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gfmofwiqk.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gmghmwlgc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gqjjsygfb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gnybvivmj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gbwpfzaon.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gfativfdy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gyjzpdora.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/ggnyhxhwr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gwquzsitm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gjymfyjuj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gdigfaxva.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gaxlvjrah.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gzrbrrocs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbvelgern.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gnwvvkjiq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnatbmmht.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gyadzjkvh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gqpqckjzw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gehlsilhd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gncwebvsf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gruxcgfqh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gkmnbnsug.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gpzjgalrc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gcockqkpj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/guolsehfq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/grdwajfpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gxmeskfrc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/ghlvyfbvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gjgvythac.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gimphjcyn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fktsv.cn/Article/details/gjqskrxum.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/glhxwrsjy.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gquwhczcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/ggidkrtsf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/gqajkknvf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gptegktvb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gkhfatwzo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gojahzpfy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gafqnaohy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gyzedvlgc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/ggaxhblfr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gjkrqgmpj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gsoohgeje.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gljxeiqfs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/grikuoapi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/grzfiyobf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/goaiebopr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gzgofvqis.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyxizmqpr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/genomarjq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/grpwteswk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gsacurrhr.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/grxznwvqt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gayreppgr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gjfxvzcmw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gbbeppcof.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gbqstkwlf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gcbqoenjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gjlqzuzxz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gfuzmwzun.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gxhqtvevw.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gdkhyjres.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gavamjfnp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/govdsunic.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gqazuvhgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gmqiogoan.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gstwdvvfx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/grbajpqjf.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gjtauwfra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gywtpnzsw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gvhwvvtrq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gllnylfuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/gedqhhlaa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/guxpaxnbk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gcnphsufc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gklsqyedk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/grizaqphu.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gktkihtrf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gzpacvjzv.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gdidhbkpn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghdekhgkq.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gqdnzqwes.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gwjqouzla.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/guariqrwg.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gfgjupmdw.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gdysiyroa.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gzyabutvd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gwvfiffis.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/grtidskwh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/ghoilcded.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gshnugkro.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gfqbzovxl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/ghnntbqaz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/goyjmwhsr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/giadfuxsi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gxhbfbhmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gmmzoxoio.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gornodliw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gzjocahog.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/ghaeismyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gclbkefqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gnrtlnbzc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/glxpdaqat.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gtcacbyfk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gdeokpcxi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gabsromoi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gmocdbjln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gvokwgmuy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gouxhaytq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gayulawba.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gxjzeutmh.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gyuxunudy.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/geyxbxzjf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gmszadowq.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gvfevosvr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/gwfgtdprj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gwpdjzxjq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gvpviycse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gwpajqqpf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gnskwyunu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gfzqikvof.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gksajzfzo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/grrustwgx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gxdlmzvdk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gttxemcub.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/glzgvheny.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gygckkylb.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gipmfrlwd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gdazoqstj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gyfdgtkrt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gujqwzmgi.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/ghfqtxaqf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gtvtglgrk.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/goptirvij.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gvvsinged.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gxpuaviwj.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gvnylsjaw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gfedwvnnq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gkbszepqg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gkxpwkvcj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gmxysccnu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gyrbttvjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gvbszuzvj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gwdgeqpsy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gjapzuixq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/ghcjgsyeg.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gfqmmjlvp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/gdirnrfvp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gbzqonhsb.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gxjnxpfti.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gwbhttoqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gyahergtt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/guqzihrfk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gacuykmsm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gbvybiohg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gtnzlgmdo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gozpgmyev.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gfpaapqdv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/guadijase.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gerndltge.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gfiajgfoi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gtubsfzme.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gvzkjnbag.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gjdnllyfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/gzmknuzew.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gknneuhpv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gumcnstkb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/goklsklug.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gezyvbaqn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gyqtkwkpd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gnyvztlty.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/guuhgilxf.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/gyiymqohl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/geslgeuic.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gnuiiilsa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gjsshrzpe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gkooryime.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gdebqdzoz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gtcfesqrw.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gxdustrel.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gblzlzuac.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzgieimyz.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwzoklvey.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gquvnharj.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gzmgijcyv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gyrkvryuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gwfdwifix.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/ggxmyhpfx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/ggzognmro.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gumkesxhx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/guswywibx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gxxrzobrc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gysyseiyw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gxouzbiim.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gmcyhtqrc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gazvjxcpe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/guyggmxxt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gkueniive.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/geiodnhpw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gwxvuckif.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gghzfpenf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/ghowcxagn.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gqigstsvi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gxrxawjum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/gstuofsiw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gjvbadpvh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gvudpmdwu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gpthmhcsy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gsxcqmbgs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gqzwfalwp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gctleomze.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gzsnlsjjl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/gjojsqjlf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/ggsfvhuep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gijyiowcn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/glwdwwnja.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/goybajlef.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/geukskhat.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gozpbcjjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/guyqunlxb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gqcqxklhg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/glvgbcfey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gkhhrzpor.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gjcxsejgz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gdnptsgni.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gzaphoidh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/gsihgroti.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gqlqacgrl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/ghjzmkeeh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gqvaoxpsp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/gfaeyvfig.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/gujubzmld.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/guwfxlski.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/gklkcigzl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gyigwxgiw.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gtartjxeh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gveabqexa.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gvubnghdf.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/glqbyzpca.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gprjlavqk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gyzekcnzm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gfxaonmgu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gjjixwutt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.yfazqb.com/Article/details/gajbmqbot.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/genchuldi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/geokxekhh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gvbnnhhbo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/grteufhug.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gsnqsmomk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gvyspqqzi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gkramfwrd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/guktuqfsf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gwdbkwqra.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gtdcxcmcu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gxqlcklhe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gatlnivrv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/geyjqteoh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gdxjbhzoi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdaeunbym.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gngnxeoxh.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gfyursspk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/glnpdqluk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gfwwkxmhj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fktsv.cn/Article/details/gjuunxptb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gpazikzaj.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gmgyvujjk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gajqqjevk.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gflpfaqee.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gwjhecwjl.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/giqrpbite.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gethoktjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gjoxvlkse.sHtML

);
来源：http://blog.vehdjk.com/Article/details/ghjctduqi.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gdssbqpwn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gpnmjwwwv.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gbektpgdn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gfcaqztyi.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/gyibsryib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gdghitdoa.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gphenoiwo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/ghxrsnkdl.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gxgjbmavi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gyinjbliy.sHtML

[Q08] 创建普通索引
来源：http://blog.bbcook.cn/Article/details/ghpqdbale.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/groatmmcl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/griiytbqk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gkepkfjsq.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/gaoshjwvr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.bbcook.cn/Article/details/gafrbtvax.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gefayeqdq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gxerdauen.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/gpoohndtm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gwdpugwzp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gxxcbjkmg.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gdxoditqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/gntdrrkmp.sHtML


<!-- 参考信息 -->