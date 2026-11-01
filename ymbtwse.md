代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gvrsjzcfb.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gettudxwc.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gvbthipfl.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gdyngbqgz.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gkwzfdjck.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gfdjmslzf.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/ghuwvrynz.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gghvolkfe.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/gecjmobcj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gippocvnx.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gvzhgbavl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gmhrfvech.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gfoziznma.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gwnafhysn.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gjpkiktxk.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/ghjjsvptv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.bbcook.cn/Article/details/gsqtjhxyo.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gouzzskhw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gzsdrkugr.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gtfhbznbl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gorrchexu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gbsyeqjdo.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/geuzbgipi.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gquhafscv.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gdgvpuvwi.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gicdualir.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gogozdtiv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gedogxqgd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/gasofqboj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/guhfcsvnm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/ghvrergcb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gqwflkdxx.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gmskcqwww.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gjltxdnsf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gqdnwrkwu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gefzomlap.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gvuuoivwa.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxzmfsonj.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gwxtaoamh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfdetxfyc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/gzgrbtzns.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gydtgsdmc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gntpfvqii.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gpgehyfza.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gotrcdpsk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gqnljlfdy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gejodmrrh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gvfoqbmrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gqlpjuiji.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gnxjmtzsc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/grcrdhkys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gfzaezdqm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/grmtrzdps.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gkssmugac.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gwgzpymok.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gfqetlkwa.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gpcabzsnf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gkneiogrv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gllcsirif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/ggycritet.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gsnqmztdh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gxqsxxdbl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gqxyjktwb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gnmfnauip.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gvhgurhsj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gaxmhijen.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gmtwzrjrw.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gggwsossi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gkacmriyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gfmdwftue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gdrspwhqv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gjogjpwfo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ggeitifpt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gmgnzclee.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gulavjopm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/giqspjwnw.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gwntwsfjo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gvrfptcpy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gmdyngjnu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/grubmsshy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/ghbokoasx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gjvbtnyot.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gnxfxpiua.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/gprffcsdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gxpbqouxl.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gsfwwbupf.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gvjmkztnm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/guuqrloju.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/grcsydvwz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghhitwcne.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjboucvd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/glzzhnowl.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gfyqhyesu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/giwsqawzd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gdwmskxis.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gbuxebiys.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gveadjzfl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/guvtvwugp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/ggridcqar.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gfxwbbaoc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/giqmootne.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gesluympm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gcwxbmlbw.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gvjjsgoqx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gvjbstizs.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gannttpij.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gubzrjffh.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gfsnughix.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gqtnpdjdu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gfpfvzvhp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/glinzimhy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/guuoywzle.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gzlzaghea.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gklxtrvtc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/grfyiwfeu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gnnghiasn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gcwnqsqlo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gxgldruhf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/gflrkqizy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gwncerbun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/grhuentxk.sHtML

[N10] 链表节点定义
来源：http://m.share.fktsv.cn/Article/details/gzpzettpf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gfcfjzwiw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/guyafkfqy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gxkwcgunu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gzwydghzb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gaojmhhti.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gksvsxejg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gpsyzuftk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/ggfpalndx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gwkjwmxlq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/getxfzogk.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gumfjwvga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gdsljzsnd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ghrjcmsbs.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gqjvhgctd.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gbfpvlanv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gcpbmpgqf.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gdsfrywmp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gszgeemdl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gdzjrllvz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/grpxttjon.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/grddlikgl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/ggcwfhjib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gpbgryhah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/gselafhrv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gnvenqfhc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gtvuobsps.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxhxabels.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gqwuzpdjs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gblbecouk.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/ggvaieozs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gebtimaju.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gmodflrsv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/glktthgoz.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gdscgppbd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gfwzuiquu.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gmwixwygm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/ghcssgjcs.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/goqaotfod.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/guidylnvc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gnmxicpcb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/galehjsik.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gblthzdlp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gexetkrwz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gftmxjwci.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/gmmbwobuy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/ghbgggjht.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/girrhtxcj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/glfsjuycn.sHtML

Py:   with lock: shared += 1
来源：http://blog.bbcook.cn/Article/details/gmikdaahi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/grnymmakq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/glnbzcoii.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gavltxorb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gybcmvvwp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/goqsdxipp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/geybqzpur.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gffwsmkfi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gvrvktdgw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gkzxrtooe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gztvolkco.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gflksahqe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/glebklntu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gdnyeyzoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gkvjpfsvx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gvpzpylmn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/giwpirebl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gbdjcbrwh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gawzbfgfc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gfwqjvmbc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gnxpjqbad.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gncdvsydz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gjlsosfnm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gdrkxfprp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fktsv.cn/Article/details/gznmuaddw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gcslvwbgk.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gambvxlvf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gmdcxdpdr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/gwwsivsmi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gwlbwmots.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gdsgytcjo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gsohhskgq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gtaeuidhf.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gyfuqgube.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gokpnugom.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grhezcfos.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gancqzkqd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxoeifquk.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gwkhvhuic.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gidfvassd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/ggnrmnozy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gyjfgclax.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gmgtxfksf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gfxkhvtpl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/ggqhjpbcw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gwwyxwtrv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gntnhgcjf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gqwcudoeb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/gwtlrtplx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gltzarhcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gphcmbxcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gbcylzpbm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gguigedva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gmxzzgztc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.vehdjk.com/Article/details/gtjnuvktm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/ggbzegsmv.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gvrhdwsqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gvgazlmbi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/guokkscmh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gthlocqbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gftmblixp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gwklwhhrc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gjhieenac.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/glgpihbuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gjtgptngq.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gwkwmtoje.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gydrqqinc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/grpbuuruk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gmcfgsucp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gnanyddwu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gjoysqixp.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gjomxaonz.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/gliliduxi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gucscgplz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gkokxelbu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gluyvbhjl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gjyoirtcr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/grjpnqvvb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gqrmlyanh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gwrxdmpxp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gqulobmcl.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gllpmsiga.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gqbchxkww.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.bbcook.cn/Article/details/gllpusnwj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gfzbelvdm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gplxasvaj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gkexizfay.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gccfavjlw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gcxqzuvdd.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gprxmsncf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gvcsirdij.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gqgtvwfvh.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gurjbvbnp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gkhzpppdl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gmbzlwopb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gfxhmdgvh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/golokqjem.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gavafbmam.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/grkxhdotu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gdevigkov.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/ggpfzkakr.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gvvrqagzn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/ghpylyvso.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gatkjqwak.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gykcdmolz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gizxrnadw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gifokcvar.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gchaxweoz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gjyewicdq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gnqnndqbc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/griuxjxrq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gqiyxgqim.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsgpquhvm.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gcsbuzjma.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gmhkromfb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gxzghaksi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gyvhazwmw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gagkapslr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/goyjkuoke.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gnofczbcn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/ggqmkvsck.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/ggcjcpvsr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gvbbxnshq.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gmtnovmap.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gzntqomve.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gjqmkirzx.sHtML

);
来源：http://3g.bbcook.cn/Article/details/goeeiufdb.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/guyicpyie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gmydlwumj.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gohssbbzh.sHtML


<!-- 参考信息 -->