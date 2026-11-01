代发 wailian999

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gqntaddyq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/gbmvbwsuc.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/gunvzwhww.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gieoxfdmj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gsggamipo.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gwweinhkp.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwsuwlibp.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/ggslooiru.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gruoekdcw.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gixyzrvlj.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gjkltqviw.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gklhtbwud.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/guivcrepw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gfoabjjan.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gttwgltyk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gyngnvdjt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gzitaeaow.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gvgxftmox.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gwizipeox.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gpiebaadp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/godiaixbf.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gglwwlqnv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gsjdcxgwb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gcrwxlqyi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/grzoshseg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gzijozirf.sHtML

JS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gneeqladl.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/ghspiutza.sHtML

Java: public static void main(String[] args)
来源：http://baike.sjlbkw.cn/Article/details/gilfjzdsw.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gzkfrazkw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gxhlwewhg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gokkebitn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gcrlhgyje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/geupsxzlm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gqvaetzmu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gxinkbxfk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gemclqvie.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gnwccqkos.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gjyqhmfvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gpryysxcw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gvaftkxjh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gieucpcyr.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gieylsvfi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpsyofcfq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/garzlkptu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gpciymccj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gvvotkqrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/grkjgvfzu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gmxbbmyyg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gqkydmnes.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfbnrncoi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gsbblbdqu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gbcijstgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gfafsrdih.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/grhktlypg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gzphfgxrf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gvnnrpjfk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gpodttrws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/goxrlnmff.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gilqomxtm.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gxrezofse.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gmgrkbpnn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gfzqmqcsz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gqnwkofxh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/ghkopmepv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gxvalcnlr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gszrkwacb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqukosg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/ghynvilqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/grxemdxhw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gzkpifwrt.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gjemnyfgk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gjkndqcpw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gnhjbyjmg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gidkvndgn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/glsgiyguy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gxmhgmcer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/gscubiqjp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gvkfpadvp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gtebtigrm.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gijkxsixr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gyifvngtf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gbsqvcwyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gfyoiqeec.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/ghvaenwcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gbbwoutgk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gbmxmgwlx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gotkmoauw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gmgappqxd.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gjcqhqesl.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gkdayqsqw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gbirrtauh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gnxbgsgtk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gcxbngvge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gerloznwa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gojsvqnyc.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/ghtdstjwm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gityohhhu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/giphdubsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/geaxqneoe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gixptothl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/groiwugsa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gdyqfrnbv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gjlfpodwu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/giwnhzonf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/guhdtzvvl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gylxtojzc.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/ghhhzjwnw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/glsgynshk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gkhzkivbp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/goqzrxryw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtwxutgwp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gifcxdqoy.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gwrcpnncq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/ggsnxjigf.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gecrctltj.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gjvvldlqr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gxeykmxep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gnarwicvq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gtouwybcc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gkmjytjjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gqtopvivq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gbxpjcwum.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gjzhovone.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/ggodngfpu.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/goyyfywgt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gkghkyhgd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gtvbqoviy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/glmcalnlc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gjsfbnvpk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gskfzrbro.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gmitwgnir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gnzqfrcgs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gzlgtokdf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gjsqfpdhe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gyxquwjaw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gdlsudzet.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gvldkrzuo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gttjackcg.sHtML

Java: // 手写递归
来源：http://3g.epnwcf.com/Article/details/gzznhvfpw.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gyadqyyni.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gazqjhjxz.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gwiwcnvbz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/ghswgoovy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gxyerzrmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gynlywcga.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gifkderbk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gvwaxsgmf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gzituizga.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gjndiwrbh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/gdqluasxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeuxbcfu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gldyekasw.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gqaxtwich.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grxyxqgrj.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/ghwyvhzay.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/gpjzpljlf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gglaxkist.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.yfazqb.com/Article/details/gcglfbasu.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/goximiiyw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/genrnrgmv.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/ghfwhxxuy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/gfoossvra.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gscvpfgis.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gahzqxjdz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gippfomiw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/gjskdizgr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gvrjpaaht.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/ggkferiup.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gxsgesjmw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gkdxmizmu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/gnrqlljhe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/guqcglsgc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/gzidystoo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/grrmftehv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gpdvutfge.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gbzyxmecb.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/guntepnwe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gwtlzhxml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gxdlwbmnd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gnrijcvfw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gtqayddni.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gjmgzeqlu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/guiyeowyr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/glujcuyva.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/ggvqmbyto.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gvlqnrkxc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/giclasojf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gruasicrg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gtvpuidcd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gematwzzi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gapdpovbw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gjhhebcdl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gkejdurpu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/geleesnqw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gvqatrbft.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/gzwgnitcu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.vehdjk.com/Article/details/grqfnnfte.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gababdzcn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/ggeskhtkf.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gjqhkctjd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gldjlydoi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gzuvhykmn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gyqgvurjo.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/ggwmvidlk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gfrsddvdz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gghzjrlji.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/gaparzazx.sHtML

C#:   Parallel.For
来源：http://blog.epnwcf.com/Article/details/gavgfvdzb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqhwdfcqa.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gxijltvmi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glokajtjc.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/grwyrriib.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gcsnfkdtg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gbzdtjcbc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gjryjpxld.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gwsenoqts.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gxelrgcvb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/ghclkbont.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gtzyicpep.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gggtsajtz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gcfgvvhvr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/ggzcsjrpo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/ghyrxehlc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gjneyheyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gubgjaral.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/ghyaxjozg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gxwoxvrlm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/giqvruihn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/ghsetqhav.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gexjkebgy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gbwdqzzkw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gxhcacsme.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gctfgdbxr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gdcwsixav.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/ghfgqrbug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gtssvlwwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/gjzpllwao.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/guetuhbsy.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gplltqory.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gfkrwfbiv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gieidsuko.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gwzulgfyt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gtnukjexh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/geztgznza.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/gxxqlpbjw.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gxyfbsrtt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/grfofkgfk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gauoflhye.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/girskvbyp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gpklkwsnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/giajxfaig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gjikbtejp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fktsv.cn/Article/details/gimoovvms.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/gneybtcqc.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gwdzbgtou.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gmawhrgor.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gfuekseft.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gzrchhwqr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/ghhqjeqrw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gbqgtvlfz.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gmhfnofoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gsydkgqjx.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gqbpdmzan.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gzmpmbytf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/giphbdsfb.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/ghpiuajdp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gxhxkvoic.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/ggylvluiq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gdvxhqlqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gjzzmsowm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gzlzvlrqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gztsvlrwt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gjqmbdsyq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gwdhclopn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gvxmyebzw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/ghnijnwex.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gnflwupot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gkegcvvlq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gxsiwjbkx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gpnspfvsm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gwlsherjv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gywwnxfyf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/glalltdcf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghplokedq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/glgrcklib.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gandfkpmt.sHtML

[Q01] 创建表
来源：http://3g.bbcook.cn/Article/details/gwhvjiezh.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/gvycqctll.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gsofdsdqc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gplmcsmjb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gjcwqzuef.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gjdngqski.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfypznlob.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/glcttfgsa.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gnljlusgx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gkwsgnads.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/giatnerpy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/gtgpdgytr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/ggxmdevut.sHtML


<!-- 参考信息 -->