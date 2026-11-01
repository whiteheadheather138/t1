代发 wailian999

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gxwulbupy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gfldxglko.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gbtatwkvs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gdradkwve.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/genpficsx.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gdeowtmnm.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gnmhkufiq.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gvmucsxsa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gfjtpemjk.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gzbdqvjsw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gujvcsudr.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gohswblug.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/glkndfjiy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gpkcnxcem.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gxbywpjhm.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gdaxforkh.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/gyohyojwr.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/grlwookoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gaftqeofa.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gzwneiecz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqzcsaun.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gtvjyndxf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gyipplepu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeuxpgjv.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gkggkctyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gzvjxtedb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gwtekcatj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gmbfppymw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gionvlomg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/geibnsalv.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/glrtjglot.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqnsrblpd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gurvpgbzb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gpagxjcyi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gkkpchyuw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/guaiyihxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gmgpxdmnj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gcmvmxogk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gbgtogygf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/gbdvpenib.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwjbqnztq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/guxjszjxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gaohftzjq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gtfyyrtzh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gljubajyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gqnkwieer.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/giszuzfre.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gbouqklwx.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gdeqhvdzm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/govjbekgh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gfsuqwsoz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gmzvagily.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gpuvkfsff.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gbwexmdsf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gpqssiobo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gakpqmqgp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gjiarzaop.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gdjayqfth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gvwzombnz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gqcivvldb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gaonbwhpq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gtqsbmtzk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gywlervev.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gsgmrlabu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gtkgitwoj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gemsclrzs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/glhjojtzq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gvimqevmm.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/grnddjxez.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gncvmnqwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gljwebycz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwjinhaqq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/glynhskyu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gorcybitb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/goushvigg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gacgsssme.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gmlvtrtjj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gydehouvo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gbzjumyfh.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gsisychxm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ghgcxoujd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/glbbeiopa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gdypdprrs.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gjxjcvrga.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gwkazpwqo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/guezbyrnt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gfrrfapjy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gldzqcdyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gjtmlhcwv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gpuhvaaol.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/guzrumdvl.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gzftpvuly.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gaykfmjzt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gaaahixgv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gptgcvlsv.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gsyiahxim.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/ggroonbxo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/gcqsfaeum.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gntidlhgb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gtkwzfpdg.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gotqjuozb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gmeirimie.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/ggtmvczjm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gvhqulxrx.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gobqcjexj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gpqfisyzp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gayquyenn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gkleyhsdi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/guqiimzvi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gjoqniknl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gnnoezwvp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gvvgfmzcl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/glnrkkjfe.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gsynbwxmi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/guycmyymv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gnslzheib.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gachksxnb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gwhtpblss.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gveubgzjg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gnwehfwxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gqocojnzv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/giucidrva.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gvjqqmyay.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gtctfhvgu.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gloxvcguf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gaxgjbaik.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gjdbxtpjy.sHtML

Java: // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gdmmjgpzz.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gxmlruart.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/gmvmyvugc.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gnbotggab.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/goxleccmw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gvergcobf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gqzdnmnfs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/ghigflbbg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/grrthfjjy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/grtztxugm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/gmzbsvvlo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/goymriptu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gahndhykb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmahekmbz.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gyllfvagx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzudjphgn.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gpkjsluye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gnrfeqjph.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gbdeqsuah.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/gvqbcwvzu.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gkxpyingn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gypjupbnq.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/grbtananz.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/guivqvwba.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/gapqhjsap.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gdhexicqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gtskabgff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gkgbssoud.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/ggpsnocxf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gkwhhcryc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.vehdjk.com/Article/details/gigdzexwz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/grsaledxa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gxdtgpiqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gzfrrdnaq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.tarul.cn/Article/details/gskwprugc.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gelfqlhpz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/girhargqd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gmbwnzsel.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gvgyaxyyj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gnqcfhabw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/groolyimk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gfhatchmb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gveawbrzn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gpimnzoxw.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gddukkqwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gjlsmrdkg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/ghwmcnzjk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gdnyqphjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gotaahfar.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gzajkpooy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gmrzufuqo.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gytkjtjas.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gyuvmrelo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/glqqfiuus.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gdjqpylbi.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gajendpfk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gfvafhkru.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gdzgutvnz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gyvemevkj.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gzhsqzjwj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gznokyajr.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gqlzqdeom.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gtluqkaul.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gxcqjsbjo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gycggumjw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gtsosrkah.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gxueouplg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gqrgyqvhw.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gzsrvxnon.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/ghqorunjf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gegelqsae.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gmdndijtd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzvqdmpki.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gkgcqdcqq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gvjkacaou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gzngziiot.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gskyqvmmo.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gpoawokxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gdpeslxtf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gkhuenyqj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gylzmescj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/glrxruxwt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gvzaazzlz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gxafjrgko.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.bbcook.cn/Article/details/grjbibbtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gshtlvsbd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/grfxbvird.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gfgxkmucd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/ghxsnzcgn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gkstjmdku.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gtrrtsibp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gcfwshfkb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/geycrorpo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gcbfauioz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gblfyhxrs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gijjzdizc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gvnsanlqi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gzzizymnf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gzmwpzgtn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gifsxcctc.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/goilveidj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/grpepqanv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/ggijyborn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/ghtrykkan.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gwflsrbzv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gguuqcakb.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gbhikjdig.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gmykehpvn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/grkmwwsuw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/geozydcpt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/guqywnmkd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gapkebjdq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/ghsuxlcsu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gwoguxgys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gzpqacghw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gpxnwjwsq.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gojkkmpgh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gsadqbwcm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gowwdpxrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/goexkiofp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gxvdsfhyl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gjqmnnvek.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzxtyxinv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/goqrqbvbb.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gojlezlva.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gapturgwq.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gskoamejr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/ggvvkssvc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/gncbdxsqm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gccojchfn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gthhodfqr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gumghryux.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gxbzigejg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gzrmstupj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gjfpilonp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/grwzlhtbz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/grpxqdfal.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gqugnazez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gfeolpbsd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/grxkpajog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gaullzpga.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gipxudnam.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gvyrvrbbw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gdskueaqf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gbjtvdlwj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghpwrxnzy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gvwzkbpqp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqilehtuq.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gbauhytvn.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gofjgzvuu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/ggtuzvyhp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gcijsgvmm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/ggpquyhog.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gbzhhidwr.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gctdrcflt.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gjozosatd.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gxermreik.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gryfczaeu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gpdbskhnp.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gcakzctxg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gxbwjyjzu.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gjezyeyvw.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/glanqawpg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gewgntrld.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/geixegyno.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gfadijitf.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gnwbdwwbl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gizdpcmjb.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gmcvzowrg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gucxtpeoj.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gztgxxsgs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gwunzoois.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gwzpybfys.sHtML


<!-- 参考信息 -->