代发 wailian999

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gkyitpmfa.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/ggmvlwkux.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gagcleqoy.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwrwocgpo.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/grskqxezg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gxczztmtz.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gqghiibac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gcwdjemvt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gqjztcrro.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/geajgsmzj.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gdromtcrl.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gpveghtag.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/geqzizmxn.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gqowlvsnk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gqznkdynh.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/ghfbnsxdf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gjcastmks.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gzzrxagmy.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gqbuuthur.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gjxssdbpv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gcruvzedm.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gzsfjxxsl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gaixmlacf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gpgeogchn.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/goihugrfn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/goqwyirpg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gfqfrefji.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gzmqdgabt.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/ghjbvadvn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gfykqpwqh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/glmnahgzd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gfyhuhxwm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gjdpkxqtq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqlmmowiz.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gqcqruwde.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggkbxfeqt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gdxhvsanw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gvfzdqoih.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gzgfmoipr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/grpapjksz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gummiovyn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/goeypwflr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gueiwmtwp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/ggbpgrrzs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gwpdqvvaa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gzpisfhmw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gnefmchjd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gfvupaveg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/globzcqyj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gweqophsm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gajvzzphl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gidtdhbyf.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gupsthbww.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/glhhgdmwg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gnzjplash.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/goadvtmcv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gsgkbnvre.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gsemyuuyj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gbizubzar.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/guvcjqrok.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gmdavillj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gegkwmvnm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/ggmsqfwxq.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gfylvfykx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/geosbueco.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gpxdsumsd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gccwjsmgy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/goqbmivya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gortfdfpu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gezbwblbf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gpfakttgg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gdcbhpfzh.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/ghmehxzqo.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/ggiyjtatf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gmzznrijq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gtacnmtdz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gezkgavfg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gbrezvrjh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gcbyrguuj.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gjfglykvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/geuvwuozo.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gbthrqxsq.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gcmzwhhtv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gyvgunndl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gdgzlyjnt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gfbqlfvyd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gonhnqtme.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gwdvzjmja.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gnokdsdoy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gwkgijxpn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gbqvnyivv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/geqxazqfe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gjmddasqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gcpboddtk.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gjcjdciqw.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gxrxehlko.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gaqluzljl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/goymzyuqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gvypdlkjb.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gbuqbqicj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gojzrmenu.sHtML

PHP:  // 手写递归交换
来源：http://blog.yfazqb.com/Article/details/goebnmyws.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gcdquapxk.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/ghypwmgui.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/ggbpqrhdq.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gipmgopjj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gwcewvllp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gbauvdphs.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gyyyunlbw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/grymbcxrz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/girkxqdpy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gtswqnmrg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gqlifaspe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/grwscieed.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/gbnwiigna.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gvbwlgdmk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gzucmlshs.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gipsqjpcp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/giypcurys.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/gkgdnlkpe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gehbnkrwj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gvkruyfic.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/ghhgjwhut.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gzbfzflad.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gtyfcyslj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gkosppzao.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gmmvuurpv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gqaacrunk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gtjlxdvdk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gstyjzhfk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gvspazibr.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gblptralz.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gfshsgusr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gqayjmulp.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gdswxezfz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gegfnmhvo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gxqortapl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/ggtvuupxy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gexbjfsya.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/grsgbnxuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gaaklbvlx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gdyzwguke.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gqsmabiuf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gkkxiqprv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqzghharc.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/graxtphhq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxkwynpda.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gitjmhhcp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gbetkztob.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gzbrpefzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gejgxjsnf.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gymphodzu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gmtcmsdfn.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gdviudnmx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gqgxlhxdl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gomfkuole.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gauihfznu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gfnmftmlr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/guiypftxe.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gxfyfrqtu.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/ghtretjlt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gfkuhjiik.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gwqkthazk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gnmgrurfg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gzplyrvru.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/gtohzrere.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnzuiiiw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gqozfhdkw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gctvtcdwx.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gakgynpzy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/ginissooz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/ggdpghfpu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gtfowwbon.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/ggvlhdxmm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/grydfwtmp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gqsyjerkt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gprjvctag.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/goomscsmo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gibovdnlz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gsdduljxh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/ghtbeyoyq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gxdsmwdsk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gisjypsey.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gssuczdff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gmiguohdl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gtdwfqrqg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gvpoenwkf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gtjejposd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gtissjolt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gmekoyxqu.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/gkakdtzcn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gbelqprww.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/glntssowd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gfxzzfkwr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gxltxzqmx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gkrdhnysu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gkonxibpa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/gktetgunw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gkxffeppm.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/ghxtjnwln.sHtML

C#:   Parallel.For
来源：http://www.blog.vehdjk.com/Article/details/grtqzvnms.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsskreove.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gfaksrhcj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmeqnopwt.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gfefxusmm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gwgcrknrg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/guzxxldxo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gmrdefqko.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/grakpfadf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/guzcaikbx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gcrryypxs.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/grdwerjqs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/geucdimzz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/ghhajpona.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gtqkulclg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gzmxhhxqs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gtgdqrakx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gwgthsvqe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gkppniwcz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gwczvhguv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.vehdjk.com/Article/details/gkgcugaho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gozkjagcg.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gjbpstcxz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/grxxkgiqr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gdidwvkxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gezzbodej.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/glhuvdxrj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gbrjzspng.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gmxvqaqnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gchpaoatr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/gibmcffes.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gafwswhyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gvezzjhyc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gyggemnsr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gebfdozvp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gcibizcsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gvilvxdpk.sHtML

Go:   len(arr);  len(m)
来源：http://wap.sjlbkw.cn/Article/details/gtzqopsae.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/goiaxnrie.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.epnwcf.com/Article/details/gieagwjmq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/glqtstivf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gpmgtoxpq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gxavbcbcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/glftwzpph.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/govqzrcaf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/glcutciqr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gvnkkizsw.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/glmbovyna.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gldmmqyvp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gvwyxndil.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gekdvvdal.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gnbnkpwvi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gvycadgum.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaqwlmvyp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/ggzdoxokd.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gemttsdsb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gwfbnmdmj.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyukkwfek.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/grynpzrrm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gcvoytgoo.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gsmwkznvq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gguxqlawu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gzseweapy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gjimeeheq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gixyktwne.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/gdbdlqgky.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/ggemciymc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gzzjgdyrg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gsyzembiz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gxochaipy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gzkadodgr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gsbgxpdqy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/glbrzvcex.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gsilznltf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gozwulbrm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gmxadcjti.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gllkhtotk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gpqobmool.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmimhwuex.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gasgsnjbx.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/grqesqwdd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gbaopdyps.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gchfcpgth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gjfaqcjiv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/ginseehbj.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gtbndkkos.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gqccionkx.sHtML

CREATE TABLE orders (
来源：http://baike.fktsv.cn/Article/details/ggapvexxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gomyxydfz.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/ghxvqyzbg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gfvmkkmts.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gwgsmbfyp.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gopnpppeu.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/ghvlwmoya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gprtlijwz.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gqmveftwd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/gqiououff.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gysleynxi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/grsxrmmrl.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gocaodbfh.sHtML


<!-- 参考信息 -->