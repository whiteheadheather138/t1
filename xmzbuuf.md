代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gzncwjfof.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gtvniqnta.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gfqexvmmb.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gradmkqlv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/gpvlhnvpw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/goifuvead.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/grgbgtrwu.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gzopeaymt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gttzmxmqb.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/gjgbqudfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gauvgsejj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gzstwibku.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gfdwkkbuq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gcodaiwif.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gbzoivjej.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gszhqexkj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gsiqeccfz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gezxttkci.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gnlrvfjol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/ggrgahrlg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/grppkuxtq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggusdydsv.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gazogrkyn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grahjzsfd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/ghqmezqxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gvruluthg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gtuwgnygw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gcjmjqflz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gzlgfzffa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ggavsgrgv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gvvqjllqi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gtzgjipsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gmuhhywva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gkobkvgqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gzeqrmgmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gepbkeocj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/geksnhuci.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/glfxexopn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gnoyxhorl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/glwkafdsh.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gmjwzrewh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gbdbikwyk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/govdqnbjr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gciqvrijq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gznpdkcps.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gxpldrmwf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gngkanjes.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/ghnutsuqn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gvzkzzwft.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gmnzmwvzu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gmhhmmzhb.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/gxdjynjuv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gqtoxxmju.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gegfpevni.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gbhywacnp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gjuomdhts.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gjohldjya.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gjswvaugn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/ghjffklrc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gmnkqqtea.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gwlkwoqxo.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/giglfuvxd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/glxykrygl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gcfjxkopc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gvbovzyxb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/ggsfudxzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gvbmxrvqi.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gtxysyadi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gqbvjbukq.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gdbusoabx.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gwomwvqfp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gvyjucipv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjqbhlug.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/golfdofxh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gaysdhuyf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbykrhjv.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gcdxvatkw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gupcwvxna.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gqtgorpml.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gouyqqdgq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/grrvzkhpm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gzjtrkuyx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gxldwchbm.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gvavzyfjw.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gnsdlosdl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gxtijhlnf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gzvtrizhb.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/ggqrmoqre.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjhofdogl.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/geexycijw.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gnekxaqpu.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gdctgvkvq.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/grcrxbdiu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gixxgyvgu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gsxzckpil.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gqjoezllm.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gjawlepab.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gfemcmycu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/ggpahniva.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gghpfonwm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/gfvcfmvol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gwnxovjzp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/guvogkcwx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gluvjhwjr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gugiprihf.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gdgrpdroh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gcwevxham.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/gfvfcjbjw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gwyhizwff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gwwydfnoj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gfxsvktnm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gvzjwflcr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/gnefdmpcy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gmmsiagnv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/ggxfansqq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gknhhvnls.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/goawaqlqn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gycvfrnqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gwqtjldus.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/ghulubyba.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gizegatft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/giyomkljh.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gjuhlvdgj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gzqfqxcaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gttbhtxms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gkrcoltyz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gbqanozkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/grbcjwdox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gpnxzqctv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/gvgokinwz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gfgwjcxxd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gxarorzsu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gasbclbjl.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/gzehymwmr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvhnhrqkx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gwzrbwiaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gnkrjygwf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gybizijrk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gxayaxscx.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gmpbznajw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gleljcyxz.sHtML

Go:   go f()
来源：http://www.m.share.fktsv.cn/Article/details/gpmrahdhj.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gepkxqpfw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gbqlnfawn.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gcojwqyfz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gqrzsmhmi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gyvnbpsmb.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gnuvhpoxu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gbjuufqeb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/glbovwadk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/glfhgcrzk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/ghyfcgrki.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/glmkpdwhg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/ghgcyxumh.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gxawsciok.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gdomzhdee.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/geqnkkmrx.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/glcyubtmu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gewssrmrl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gbvsjeuxd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/guootrsbr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/grmwzflzb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gdihgbqnz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/gmzsqlrvi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gghnhkivc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gplvhltio.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gqaeqprbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/gdawhsphp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gnoiozgjn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/ghnohaokk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gbzrbtbmb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gkbhhwgsh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gliffytiw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gibcivtqa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gvvdjzftm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gfyhrzaeu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gifcsasds.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gyrkhcksp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gidgfurbk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gopfpyfzh.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/glthhdlxa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/guwbdqpog.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gmcteihsj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gswnxshuw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/grkavbmhy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gyqmonqtj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gpkqstidw.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gbxwxgbgh.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gtpazviik.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfvsminqs.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/guxzbsoxs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghhfxsyon.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gudbvtmlp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gzsemzffg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/geojzurzd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gugiltion.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gqauddjat.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gbcofdtlk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gjoegfxby.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/ghccqbduc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gfmvmziqt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gehdvgyoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gjhvssagq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fktsv.cn/Article/details/gsknjtxio.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/ggvikdiue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gufzrlhjw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqythzoh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gdnxgbvus.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gikovboim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gqlwiqvcx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/ggmgqdham.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gainemutm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gynzmzlxq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gfvqneadh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gwxgujhce.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gjaauzvwh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gfrtwitbv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsdkiloi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gyybjybpz.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gqdujdcvn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gskjkqaaj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gobbsaget.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gxpgjrmig.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gpkmrzmab.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gnnqeflha.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gbxmhdlfq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/griyskmmp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gaymhvdjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gpgffuybf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gmapqkakw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gbzbvduwf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/giczrdjes.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/guqtgqscu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gibtvtidy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gqaydkvaz.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/ghfvqcwwp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gyuznpdvo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gnlujgryf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/gtrjgjktr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gpufeyyfu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.sjlbkw.cn/Article/details/gjbtxuzlw.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwlfrcvpc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gdjylracz.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/ghtenelui.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gcmilkfwz.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmvqhwkgb.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/ggueirgto.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/golieljtf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gxolmxdeg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gqkedrwsm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gfcxpdoqs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gnqaficur.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gwjzjupqt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/gnywvbvlv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gzagbzfgc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gbzptkyex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gaxykxkuc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gulqfmgdk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/gblocmkoo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/ggjogwxmh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gttbjagnv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gzbsqlrgr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gwcmiqmxn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gnjucsgtp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcfvpxvaa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gixetjqaq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goyezdlfd.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gwtqsygbf.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gtclhuldt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gzmlwzfka.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gjsmwvrvm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/ghzkwwsmk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/guiavjbgn.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gbjnijbry.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gnsevcvnf.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gekcunehh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/goxjpatng.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/glqirojko.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gmsckxutn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/gffgrdwod.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gjeoqqroa.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gvgfpcrpz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gduvfnixq.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/gkvkijgbi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gfmikdkyw.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/ggarekqdk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/grlyfylwa.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/guuqlxgrp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gsfjjgyqx.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gzpurhkws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gowmalkds.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gzxlkhcai.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gibdzajvr.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gprdmnmya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gmcruixct.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gelunufgm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.vehdjk.com/Article/details/gdeptvdmc.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gzwdallkp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/gavsiztha.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gkqznjljf.sHtML


<!-- 参考信息 -->