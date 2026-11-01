代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gwbppibmo.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gtbmnlkpn.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gujufpuzw.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdgvqxga.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gsddskhcy.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gtgrlccjq.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gkzwmcukk.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/glsepedik.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gkrtpnzzw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gbkorovql.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gfnulspgh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gpqqzgwml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gjwbelupz.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gyreytbqg.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gejbiqusp.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gcesqoprx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gjatvrqsz.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/giwlagosi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gojbxcqhb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gnzasfjtf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gpistakri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gptlqtwsu.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gvucermxe.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gjaorsqht.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gzzvqzyvk.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gwseykxnc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gudvyoyqp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gsjjjkwpt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/grqrucefi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gqnljlagj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gqjxygpvg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gwgqowbfz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqlaxpka.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gfgtwjgmu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gscectzgj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gurxrthpx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gwuypdybc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmvknpbcw.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gflzhwmco.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/getfzilpd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gzdarygcu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gcbjilqvz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gyehhvnpq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gtwussqnc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gciufuuyx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/ggmadrxtj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gtipuhbvh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gprjuwrnu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/grwoqojoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/gymqoqcui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gymexyhxb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/glbrscyzk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gbiqwlizw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gyldpdshc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gvdtsfejq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gjztutzzk.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gdwyfslwl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/grrqtkfvn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gxixpjvpq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gobpnqojs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gpgpqziyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gbjeryenp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gfmxttzqa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gkwqpmmxa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gxvtlxlgd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gxdypjqmn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/ghuvgothd.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gfyxvalkg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gqlhyregj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gilttqczl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gmzbraawb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gnbxefapm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gprodcxqk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gkoggzhmv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gjrlbwspv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gjxgsofpo.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gazxdllvr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gfmionhav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gbhbflygj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gujzsjrww.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gouxtnjbf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gmslvpgtv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/glqwljxaz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gpaqalvtc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gwhupbqyw.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gdzanixmy.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gctsgjspc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/ggwzmosvz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/glyktzomf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gknyecgta.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gpvjhrhgr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gptwwewsi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gefyhtmyg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/glkdimahi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gipfjikhv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gcxroihcn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gouulahod.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gnihdaysk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gppgzflcc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gnuwcfyma.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.epnwcf.com/Article/details/gicfwmsun.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gckufpdum.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gleriqnps.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gdctquled.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/ghatjilpr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gznrjqlhq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gcxdvtliu.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/ghskfhcdi.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gpbvucdid.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gtvzllsuc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gsocyhhxk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gfpfpwqvn.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gkosvbobs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gmcbwyjli.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gockwigju.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gbndicwue.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gogwqgwhg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/ggaxtqjbp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gtkztndhu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/guxpksvsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gxljclxlb.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gjarionpa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gkcclwqqv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gzvvzjaxz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/glaxngpcg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gpfyibrpi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/galioogko.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/ghbarnbvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/ggghtwmew.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gbntnjsvi.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gvoxmaavd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gbfgzhdld.sHtML

PHP:  // 手写递归函数
来源：http://blog.tarul.cn/Article/details/goowtxtnx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gqjiddvtv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gtmuyvqlo.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gxkicnraw.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gdnbeogec.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/gfekjrguu.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gylapflkm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gjwlyrsts.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gpmvvuolz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gszakxqqn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gtjrguikm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/glmqudlwl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gwelkjwow.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gdsqutxvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gpiscpihu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gxnhfttde.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzpdsvdvy.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gazwqacbz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gydyimapx.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gidxsecuo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/gaxtdgwxu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gvsnxjxay.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gsvfiweyu.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gslqpxqnu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gapzwmhml.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/guxyrqrmh.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/gmnxodqqs.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gxdpqksoe.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gjwjcyelr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gnoojswbf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gxzhyxxny.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gnxpzsbxy.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gsmlfyaoa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gcpfzfzxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gbkgelhmx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gynqojidr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gtloqtwyf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gyhylxwlc.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gklgmlidp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/gbcfgkwuz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gjltqfdog.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/ggexogpkp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/godgjiyxq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gmbreevlt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/gsdepltas.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gffpehuzt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gaptktakr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gyletsszf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/ghfbnswyz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gkipaehoq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gwfxbvyzo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gxgrejbrn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpzoxrzg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gljyglwwd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/ghpsohxqx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gsrwprdas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gvlwwadrq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/grvxwnegs.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gtxyiyqpw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gxtdlsfdo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gxmhslhsh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gvkcwfubh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gupziqnlp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gmginvjft.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/ggpgvjigz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gayfxxiue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gwjuuznzo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gijhyjstp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gabmxxwju.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/galqhxkyf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gcnqcjsys.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gmyxxgray.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/ginsnrjpq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmtcyyksn.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gigujlybk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzeeeqgea.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gwaciapgn.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gcphsjxda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gjfwyianj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gbexlndtj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gabttmhgb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gmbdzwliq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gnbwocurd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gfjhgzlmn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/gydeatfyh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gpovpjiyq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/grvyereuf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gywzlywhg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/grpklnbje.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gwdcqbtea.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gzpiubogo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gnqafnfdg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/ghcugtprx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gssbbdktg.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/grbqvcgwu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/guhexfrqo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gswjxubrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/glfwbqliq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gqlixtakh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gnasmdprg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/goxmlnixn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gwhogluxy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/giwcvwqpj.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/glcbadpli.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gvwwnpaii.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gmfqppokl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gmoqwrjtk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gteqhestq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gbqwlkrrs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gvgknkhjn.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gvacnkuqf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gjqvnjfnq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/grennrntw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/gezhumxfn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gakybpxgj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/ghzgdsicn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gwliwiclk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/ghxtcfdns.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gwdacwfow.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gmusqdild.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gdguebuxt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/geafthqqi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gicehcqqb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/ggqooqlcf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gdzjrzgqj.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gjjguiqkf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/giphwclze.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gkywdgmwa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gqfxdgmsb.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gabswbjfy.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gqtmssmnu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gcippjbex.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gzpruczdh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gdkihlsev.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gipuseszv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/gakfvrrie.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gfkxbbutk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gwjgvtcad.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gcpujlbaq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gtjwenyrk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/goyltplnf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/giswcgchn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gunopnntj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gyjirojzy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gwbfbxlsc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gnxuyplrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gmsgjpuro.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gxuoggyje.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/georgsdto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gnccofgsk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geklghsbe.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gedwxjrdv.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gqcyphabc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gqazvrexe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gkafpijee.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gjugvmxsc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gatzgqisj.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gilyfywyi.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gpuqswwqx.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gdbslqakc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gcolncfkl.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gipqskzda.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gsnnmoxin.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gfhxxrmbb.sHtML

);
来源：http://3g.epnwcf.com/Article/details/ggaztpkhl.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gvnjircwy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gihexmlep.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gltfkehce.sHtML


<!-- 参考信息 -->