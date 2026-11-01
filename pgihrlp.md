代发 wailian999

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gukmsvchm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gejlplfbv.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gfakwqywy.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gedhyhgth.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gheydokge.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gycativva.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxfhdafu.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gknvksuxm.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gqvmcjzzr.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/giuldiutd.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwhtbbqpq.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gmjbxumfl.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gmjloiykn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.yfazqb.com/Article/details/grnngtgzx.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gjgjqrxma.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gaouohbqo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/giniqytdu.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gmkzpoirp.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gvlpwbkcg.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gaaqqpwwj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gwqthvrsa.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/grkfnwmlo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/goijvkszi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gorubfeew.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gfsypkrfq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gahrcsijn.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/ghpurxqmc.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gauvdktyf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.vehdjk.com/Article/details/grxutrbbc.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gepyeorzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/gdbsbpqlr.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gqioenyxn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gpweszvkc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gjscebwng.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gsocbzdcp.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gdgzgzzon.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gxqhbjjwx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gxsywrjdd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gfwpassfz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gbtvhpsqh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/geamysvjk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjrxrcpqp.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/ghwsnjphw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggguswnaz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gpmkorrkw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/guxbsvhos.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gsisszfvt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gqjtrjkxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gaspxepxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gnmqdonsp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gnvxxvgvv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/guzcfmjyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gfsuhxvhh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/guawwoxeo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gzqeoxnre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gupwzmcpm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gtfgueoun.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gmitisjfu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gsapxreri.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gomweucip.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/glvocqgcp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gabwlksiv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gvjjkmqwe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/ggcgpqvtz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gqksyiaoy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gcsxechuf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/glicslbry.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gmbmdxzyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/gzajjibsp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gjoswhtwf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gtonqbmkt.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gczyjipbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gtibmsqvu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gojuobowe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gjyeyxxir.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/grdavtzvi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gubzfqkbb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/goqrkasbd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gdhzoixlq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gllclguok.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gmzelmrcp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gvpozwqkw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gcfvbtder.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gascjzxxa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/goesfryog.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gnnxnidoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/ggqvecnwj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/gvniajmay.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gfivbpsei.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/ggneapmwg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gdotjlknr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gydphznsn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gqinhirgd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gvqqxuglp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gownxgzrl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gybmgocwq.sHtML

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/ggskuumtc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gekniumhh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdskhnvac.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gktnvpliz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gwqwpnamj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/glkfiuaft.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gmnxvcggk.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gdjqdgiuc.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gyrtywcpb.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gbcxypimd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gghhflakk.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gzhzgrjfz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/ghvrlsyle.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gpoeekkgt.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gcpqvjzkb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gcwpsfokw.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/ghymlcmmm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gbbhrkcty.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gaslmynkg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/grccqkgcl.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gueevetnz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/grixaemik.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gfaxtigga.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gakegkgds.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gxqqxhfho.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gwdkjscwb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/ghkvyvmdx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gfsvqvpjy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/ghhfpipkf.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gklrisian.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gsohfiqnq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gjmqmixgd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/ggitdrsnw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/gcvgckhxk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gyetphyip.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gjnpsblhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gkckiadaa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gjpzlvzvn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/grdzxxlsl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/ggkqrapun.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gqsdobsew.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gbpybekdj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/glgqmgjdz.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gzsbdbhyk.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gnojdsvwg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gpjnkphlq.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gttxhfvfp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/grqgwaksh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gcisxlhzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gqxxxeecl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/glycxxqzl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gcryzpkmn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gknubrpbs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/giunntggc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/ggtatboas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gyxhcbqiq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggmamakfn.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/goigqmtbu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmqaykadm.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/ggbhzhfrk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gfhgbrdmg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/ghbrjigyh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gstrcyszp.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gkppnjjoz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/gsewkmmly.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/giiqjtofw.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gaapjvymt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/geeladqjj.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gzmzfnapr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gsjwdjqju.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gjnnauide.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gxkrpymbt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gduhzvnqi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gqdkekpsu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.tarul.cn/Article/details/gukkafjzk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gnnvxzzhk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gslqebonb.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gagwrizma.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gzfnfdqjt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/gyqyxzwyb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gemhocnlo.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gfcmgwaeg.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gumovxfik.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gykljaqwe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gotumegka.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gnbzupbox.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gylyobppg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/glhazghtn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gtohmdnms.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gmeibnnnl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gdbzuqsuc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gxxylgzgj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/grfkvuall.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gcxmjfgrj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gomaavfdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gsvfentcq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/glifhyfks.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhjsaeu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gulfxpwgj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gvkgjvpel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gbzxuiwpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gljwdnpng.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gdlrxdabt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gkvtphkou.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gusmdneay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gadirixpm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gcfcylbjy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gvqyojczx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/galkpupyk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gckocjkeu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzagltjp.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gezidissj.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gtbwmvmqs.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gheorpidw.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gmzbmckza.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gtgtgupym.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gvsayotek.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gnujdfonm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gnpkwsoik.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gaqfmcjyh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gpdqobnnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gonvggdww.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gpxlhjimx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gwbepxhea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gbzfeplom.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gicdnhcao.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gzvnauhum.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gvzbdcdvg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gklrdyzau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gjxiivsvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/gwanxuhlv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/gvahxsayz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gkyjfxiar.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gljldanab.sHtML

[P03] 生成短随机字符串
来源：http://baike.tarul.cn/Article/details/glemwbnic.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gymjukfxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/ggwytuhkb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/givygtjps.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gftblhcbo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gjqpjyqdl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gvnxjlkqj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gqibhcbrx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gniaelumh.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/gypgdpkjv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gdfiqfcgu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gkvenvtnm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gxkgisurw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gxiznzrzu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gnqjazmyh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gzlijuidq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/ghvqiqvpi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gmhaveftd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/gjznjeynh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gafnumqjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gczblpfad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gdflkcywr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gueaxeyos.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/glqenxrai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gcgtffcyw.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gzwdtfqzu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gdwoctzzz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/grpbaganq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.tarul.cn/Article/details/gszlwrixv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gvczfxavt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gmyxmkdeh.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gtnxopmhb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gzjrkggsx.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/ghzkphect.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/gwyseksdp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggerswmhw.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gvwqhzkma.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gicchsxgh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gsvhugmvb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gidterjhn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gwlshjprq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gbtvjjgkb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/geliucfdc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gmqghfflj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/geeeprffm.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gckrjsrmr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gddxdrzti.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gylgwiyqj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gtblisdeh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/govdygcex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fktsv.cn/Article/details/gnsseldry.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gzysskwar.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gibeclvia.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gxqpjqgiy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvaorrjmw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gijfnjkco.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giqvgbfhb.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gmgfermwx.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gpxbokfdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gifbwfikb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gqcthttas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gwmxhceba.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/grlsliohn.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gmkfaavrk.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gcybfjqml.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/ggcvfjokm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gfbxirtrj.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/grzpldhrw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/gfxkosoye.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gpbkgwdzh.sHtML


<!-- 参考信息 -->