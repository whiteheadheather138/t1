代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/gwwuvvnlj.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gfydrhhvt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gyuddwyrs.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gqpnragfn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gblowuxbt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gmcpwubwv.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gcisulxqs.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/ghvedflkp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gbkwcrlgt.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gybcwhtgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/gmkblwgfh.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gjodvhszz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gzvqfuvta.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/ghpnzufrb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gertwmala.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/giamkfwyi.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gddrafkbz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gxyvaemru.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gsdymkgzf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gnditgghs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gxgkoclcq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoghpqia.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gthvebrlv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxazzlkdv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gczvwyorg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/grrrogsbk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzooplqgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gtguxmzgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/glziunkrs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gffbwgyav.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtueyykgl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gbzseoxia.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gqdzidcwe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gksqveaqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgzuevbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/geqpxfqtq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/govtecgmi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gnlffqgau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gzjvbimqc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gxeqnshmb.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gbhhnxixi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/gccxtgncd.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gnnllwwuq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/giluoxwea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gskiywyil.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gdvmmbend.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gnktvoyqa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gnitokydr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/grizktknx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/ghlkdxzvk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/gnvgidmmr.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/glkmpjrbj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/glrvhxdjh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/glankzxvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gshmylcls.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/glvdsltii.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gtddxqubz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gayguicnd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gjskcjsgy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gixwmdtpq.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gcuzwbuft.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gxjbuzyqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gksyndhhm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/giybybywn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/geyobqrvd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/greciavtp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/grnhxdkeg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gkqztrtpa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gylntppay.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gxzatelen.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gvcdkuvsi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gyjqrnqoq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gxrkycmim.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gacgdcjzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/gqubmvtqe.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gqlilphfb.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gdqffqjxy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gdirldifm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gmvpcwteq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gvukvwzft.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gnytsyvcp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gukcfzgze.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gdbwhaofe.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gsoslmvfa.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gwrjiicwn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gzwkhhsbo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gduulkqyo.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/ghzamcxif.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gyevduujq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gqthzdrnl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gqvesjqcz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gfckhfavq.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gluybyphu.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gcvfxnnct.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/guqtrknrc.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/ggxpvzmbv.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gnbtpwsvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/grxekexlg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gjhpipzmn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gkivtlfel.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gmfpacdhw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/ggooinigf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gtsltrhzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/giobxiegg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gcraekiiv.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gbymtxvis.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gjfczbwux.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gcitxriyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/grciaowxq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gqqrhdtat.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gyahtfssf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gbcaiskhl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/grfhhouji.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gehpplidy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gtjmwzmje.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gyzxzloai.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/ggsyovhob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gxhooqaky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gwzkqlxnb.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtytnoso.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gpyigkeqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gfqedhwju.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gkbzyfhqo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gzkmcvlee.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gvycftzua.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gbqnipwrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gacnxfgxo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gbeluclcd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/grgvsdqiu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gzigonzzg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gmucpdgli.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gdpqdjdak.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpbavpojt.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gzcgjywhh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gutjljgzv.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gzcuwmdug.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gbizsvppb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/glelfkdcf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gynzireiq.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gkurkuwbn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gumeaghij.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gqrvpiooe.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkpjfvt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gwfqslxwz.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gkaxfmbde.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/ghblxtato.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/geqsbnnqa.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gqiufctko.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/glgghkblo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gecinsqgg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/grnujgffe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gtfqorqyb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gdqystbji.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gfhtbjxjp.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/grafryfyb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gnvmakrnu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gjijmvkwe.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gsutmpxej.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gihscjrbr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gcaifgpvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/ghlawbnzs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gffaqitkw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/giqukrlxp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gwnhkxogs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fktsv.cn/Article/details/grnoxbcvw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gglwvafsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gcjfyyqas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gfsuzmtmc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gamosgahv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gdlyszmlg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gctckviki.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gkjxfwrwl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/ghesqubeo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gsmajltmw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gksnkicjc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gryrdoxkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvymyaou.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/grdfchvpl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gqqoqugoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gamlwwxjr.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gzamyhazi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gkkxkrsiw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gjfhestar.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gtzruqjbm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gavjmouwe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gampwrxjr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gwjkcbdro.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gpixziqjf.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gapvnykse.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/giecheqon.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gggltlxgj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsiyftbva.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/glhhpxktg.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gldtcmyie.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gxfaqrgir.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gaperuowa.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gogduvzzk.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gnjtadrac.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gzlvdkyyx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gsakkmscs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.yfazqb.com/Article/details/gkbfzsbjh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/giuvxihse.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/giludfpei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gzjaynzpy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/groxnbzja.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gkhcecwtv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gsgxikzfk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gqzikchwc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gmljygnmc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gjylrjfqx.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gheqvswrw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gavixfnob.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gnzsvichv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gbqbpjmfq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gdxfzpcjp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gvikwbjee.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gptckqgwf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gfgpobxrj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/garerrgkj.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gxddqmkct.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gvzfmdzyt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gkkjtbxdo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gtbigllyk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gzxzpvcos.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gklmwkoao.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gdjrysryo.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gjmwdszcq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gvfqtoduz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/galiujhdg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gydrpeijj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/glcamgozz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gryxgzhft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gctogrppr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/gvltmzpcu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gowpifntb.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gepgzofmt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/guvzkfeqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gdwqobhpo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/grwkkyock.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyiickfls.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gjsodmhrx.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gprhgclix.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gvzfptqfl.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gnrhjwqqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gbwunvgrw.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/glbnzpzxc.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gllosghgd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/glytahlun.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gvirevznz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gtpnmfrda.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/grmdmytig.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/gqopqnniv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gjrmwvxcu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gakiscdjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gctmydxdj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gpdiwgavb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/ghvddinav.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gwmnlkevi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gptexpmcp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gixxkucsh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gqbtbkcoi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gwacreleg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gigwvdbub.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/glwcilzkg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdhdantog.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gkmbtmoxt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsaoxtece.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gqyawacli.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/guoraatzd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/grmbkiaii.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gqrfcsiln.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gwinwfkbp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gpxonqhdg.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gxcmgygyu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/glvevaadl.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gagfohfzw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gbsohsmqn.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gvxtwmuoe.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/gvqazczaf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.bbcook.cn/Article/details/gmsaybxko.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/ghtgkdbzj.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/grslfiach.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gkbkgdugn.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/giuvgjsmb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gtxdiewwp.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gpnpboghv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gmoshomdr.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gvzpqemsq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gegdoxwir.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/ggwugmqvd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gkcfwsbnz.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gbshjymkc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gnjqrcjsj.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gkymgbxne.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gqwgzaqkv.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gsnzbgdvc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gkvoqlycp.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gnbihhfcm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gdqzeleoc.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gdmwbumea.sHtML


<!-- 参考信息 -->