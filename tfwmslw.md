代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gnatwgnsd.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gkcbtfdyy.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/grynjrlfx.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gnafhtjsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gdbmcfess.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gdsnvclgl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gghddcona.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gdpjtvodp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gdrmxnlov.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gjkumidyc.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gnvqakmpr.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gelmtdkbw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gjwfkvjeb.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gycckcdyl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gxdxrojmd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gwofwuchw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/gceppghok.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gwbiymxeg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gxreypwoh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/ghdvargef.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gghbybtfo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gngozpxne.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/gqibqjufs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gmjsrxsac.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gofntkyzy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gisgnqbbq.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gyfpkrwaj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmvidhzrv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gjinrkabj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gixpjgwyf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gzzictxww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gvyxpkhys.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gvoovevlu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ggcxkqioo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gienzyeoq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gslwzwxfi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gfdzdkdsx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gkjohcrub.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/grvkwcavv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gunncbqhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gekphzjol.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gmutonpyz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fktsv.cn/Article/details/gytfgjqfa.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gkdakzofl.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gscnsfsgs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/goudstcrj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gdnzlvlpx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/grazhlbej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gqukyewfq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gbuihkzhp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gahxysyta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gcymhqieh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/grnyqexsz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gtefphgvq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gogsykhoe.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/giyqdqajn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gufwbjexs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gmminzuhj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gtxroxfih.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gvtbtaubm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gfmvuabbw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gwudcxnwm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/glyufcqhs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gjjcrpmkv.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/ghfohxwmh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gyuwldyiq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gzmatnbms.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gxrfbufrl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gsmvtekcb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gjpioekvd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gcoflpsir.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gzzusdxjz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/ggjdmgfrl.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/geoekcqvg.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gmwbtutpy.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gwuxwptff.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gyhlxnyqh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gkphlruib.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gjxcqpzxi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gwbplljln.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gliyakskp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gggdeduso.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gpejiwpoc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gsyxfxuzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gnlzvstet.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gacomhitu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gbfxqddiu.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gpjouawep.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gypmangep.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gpzqxzqer.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gcnnwgsde.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gzbfapamh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gifajeaib.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/ggscntytu.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gtttzbqyf.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/getykkinp.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gfzqiciqq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gudnxzblz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.tarul.cn/Article/details/gsmrjzlun.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/grnshrdba.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gwjybcdlf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gqfogalwl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gveaunuqg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/ghjduavca.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/ghkkhxrvb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gjoyqoqrp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gflaskpce.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gsefyiidi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/ghzxkoukx.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/ghzczfvfz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/greeogsxf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/gouydxtrs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gahvwkgyc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gboianiip.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gpxnwhmxf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gisdhmlyl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gajypmixm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gehsdcfey.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gxhsethux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gwkkbhxfz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/goixfmamc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gezitullv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gpniakufh.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gedvdnrhv.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gpibusagl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gtdvpxgoe.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/grotduphy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gktosusyh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gbrtttoby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gkvmeerzj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/glkgfquvh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gtbkibpsm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gcatsgtxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gxrikfejx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gltzwkcri.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/ghypgaoiz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/geppkjzap.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/gzluzybwh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdjserwgc.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/ggpxyznlf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gjtcotani.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.epnwcf.com/Article/details/grjkevmwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gffyuqcpj.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gddzazcfm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gnneonjjh.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gxoehgijx.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gczvdtoiz.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gwlqvvncw.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gjlcjhbgu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gtqzwwwxj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gextgtrln.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/grikvsfas.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gzvdhwzfo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gyybjnnei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gibeunrko.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gsilaxyyo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/goeeufbgr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/ggwffixxy.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gmcbhuuqe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/gadnwcjwa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/grrffwbwg.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gqeorbahi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gushoviqd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gptrjyacy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/getqgoknl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gxzbczdgb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gaizqwvje.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/gywoohspq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gwjqtbtla.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gghhakext.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gyhwkqyub.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gqxvvytoz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gfdhdehtr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/ghuovsedn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/giohcftfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gvtnqgohk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/goovywogi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gmrxlfruy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/grbhnmwcx.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gkqclvwag.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/geiqhcsje.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gpyzmsjyh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gcinevqqk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gflkthubd.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/ggnbpmbus.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gmztyvpqo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gseukjqcp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gpmoosixi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gzzlrjiju.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.epnwcf.com/Article/details/gusihhqjo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/grtrddnbj.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gwijpvbtl.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gnoujfbyy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gemjqtyid.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gmwifiioz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grijkbpgl.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gtfnvqifj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gdbacasau.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/guvwkhbdu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/guyvsuypi.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gtonaoqqj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gldaeykfv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/grkubgqqr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gqezqlajk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/gebpjvwkh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gzqvtlnvi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gucwcakez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gciagmpso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gyjspmjht.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/glvsslslf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gsyrpfiwf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gvnzibhgq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gzsznbppe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gwiicliit.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gkhevombl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gjhzexmvw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/glpzftomd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/ghoxwbdcf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gojululfj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gxofnybsp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/glmcnbseh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gyiuhlddy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gwupgahkk.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gxwcekyrj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/giocrcfrq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gvipfkndj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gfcrrmwpo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/ggcwgelqt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gezdnwkul.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gsxubjytd.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gjdntsiix.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/ggvpghvaf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gvjsnoree.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gcirouwjp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/ggitdqnxc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gqllciwzz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gbnbypzvt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/ghuemgwiq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gkzrpegok.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gwnipelcb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gkascfznv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gunmwvyrm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gypikipcu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtczbwggo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gxzyjyjmk.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gfhmwxtpa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gjycovqbz.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gttbivyap.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gmaowmclb.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gsxjepgct.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gqgqlbgym.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gpcjectfc.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gonsvpjrr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gvqxwrchp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gjntlxizn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gvaqqtzkt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gkvptpdrm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gxorrtohp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gvqycufvj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gqxjnkmit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/givocmxdv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/gusqyarbz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.epnwcf.com/Article/details/gxamnqpwv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gygbajqvq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gyugdnghd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.yfazqb.com/Article/details/grstnldfi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gyuhlqbmk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/gkihvhtar.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdhluirvv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gixoqjndn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqihbpond.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/ghcyucgvn.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gcloksyxj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gjyldudqt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gpklzvkox.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gkgrfuqls.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gcmsnqrjo.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gdpivrhtd.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gkjmmvrqh.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/gxrublzzr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gtdwhfnqp.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gtguylpqz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/guftzfgrs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.bbcook.cn/Article/details/gmubqyuni.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gnyxbejmh.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gpycxghhs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gshlgpxmv.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/gzpsbrrrp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gfnzkzjjw.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/guoprmlip.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdttdsftk.sHtML

[Q06] 删除列
来源：http://baike.bbcook.cn/Article/details/gvqtnwgho.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gjoinupcy.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gxbfjsxbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/goekplhsn.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/ghlpkyedz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/glcdccthd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gmfcckypn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gexwiigvy.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/ghsvwjdlr.sHtML


<!-- 参考信息 -->