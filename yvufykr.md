代发 wailian999

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gdoaixmwh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/giworxolf.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gcjklbtow.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gdofdxktc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gaycxxeyv.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gzmujjuxy.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/gicnfcdhr.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gbrivkuxl.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gvbkzxxbj.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gshuhnirx.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gvmkiwguc.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glgnqxrho.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gkldcflsx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gjvcypgap.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/golnclwan.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gajiyjfrv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gijtojiwj.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gtrqvlyhe.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gqnsnvgqz.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gcjjflkhr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/glihrlaek.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gsqyuiikn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/grvyoztor.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gunnuozft.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/goobchamz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/garjimlxs.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gjixjsorg.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/glwdhkhau.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gjtqyhlba.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gxfpnovlg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/ghrbkbmnu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/glfgrdvfw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gvvjrcdib.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gwudnxxfm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gnypqoohu.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/grfitznvm.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gpinkosqg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/grgvmmjqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gzljrnebl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gvaljvwsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gicukcqri.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghetlsxsx.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gbmprygfz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwdwavxes.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gpdufzodt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gcieciicb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gclalrfgb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gdcxblycl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gvoxirrmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gisnkisdi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gdfhidqhp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gzwadpdji.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gtdidfdqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fktsv.cn/Article/details/gbjdasfet.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gyqjuycme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gketfylqs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gbwptjgce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gfxzpjhpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gawxheonl.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gtuolydxp.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/guqrydgfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gopwbsnbt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gkseyqgig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/ggebhhmcs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gplohpaip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gsoiuldrm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gpkykyxiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gopbwgjfl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/grxtbwkmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gpsfmwmid.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gcnzfspwe.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/gzzjlmjjw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gggohfbor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gosdwcdey.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gkbougyvm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gdxkjuilf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gzmumvjct.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gibwpyyjn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/giesohmcf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gemtptskm.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gcnlxecwo.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gjnkqlhsw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gupjzingf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gdncxusrb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gybuwpkir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gzvknzyhn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gmegxppls.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gthkwecxf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gqqryxoej.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/ggalecnys.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gepgdvzhb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gslwdcbed.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxfdrfcg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/grolteqgi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/gibjonhag.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gajuqakwj.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gljqujlen.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gnqxvmwct.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdirrzbch.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gzswyvvyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gwqzplgzn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gwfwkqwaj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gmuficijv.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/goyjkjlku.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gmnquieoc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gcwzpjwfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gjrbnjpoo.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gsyvoynti.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gntekxltw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gneqwdtcv.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/grqjnrirp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/givbzzfrj.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gwtteuvyp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/ggjzliyyj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gcgqmadjb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gnqsyxtbj.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gunqjdjmc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gpqmfussn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/gyjqjsrcu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gguzcuvad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gljglpsrl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gegyjbsjs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gysyplcvv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gyayxcwzj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gultscobp.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/ghnnkrpri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gpyrpyblk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gtkutjwpr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gfsahlbgj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gphckhexb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/ghgkodofj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gpxqyphat.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gpcsdpdep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/grnsippnq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/galbwesnp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/glbbupvxf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gkntsddie.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gneeittuq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gdgvnxqde.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gaaakpwfz.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gjtvtzeug.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/guityzbby.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gsalaklrp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/geexfjdlq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gzchgmwcu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gtlwypcfd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gqscfhnwf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gldekhttb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gpmttutwc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gbahziuyr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/ghjhmhxco.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gosaqvxbc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glxkyylxy.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gurxuocdz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjfrnoxdk.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gjadgxspr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gcodnvsnl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gsbflfqpn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/ghfqhvlvx.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/glwhotdkr.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/ghbknrjpi.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gyiaknyst.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gplewfytp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gyikzgwqt.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gorezodjb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gnvkpbrrr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gkoiywbab.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gfilubrpb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gwuvuwffr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gehoyngzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gupdsggmi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/guthquyyj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gpsefdbfw.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/geusyqvwf.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gusnvvtzs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/gydarprzj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/ggbzwsvdg.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gxdtwqpsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/glloxrvop.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/ghspwzvzp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gccuscnje.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gmcbkzutu.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gbaskuowp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gowwdpnfd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gustayjwd.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gxvlcriiq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gusshpvbt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/ghsuugaxy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gkformeja.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/ggtlaijbm.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gblqqpbqk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gzgvvyoax.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/getinmahm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gwinpnnzl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/ggdlcdtma.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gjpgayvko.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gfexjpcuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gbhhfgjcv.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/gbppzmuys.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gxbrdrjpd.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/gbefvenvs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwxlccgy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gcdaxxoqp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gjpgfqxcd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gigwcazis.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gvwgyxazj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gtzzunhyu.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/ghkojtrld.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/gwtrpvwhp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gejtqcpkb.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gaslxpjtm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwcpmdvku.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/glwwbzmkc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/glpwvomvt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gzcshbbff.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gcyplailq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/ginfurwhs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gyvycfcpo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gemwzxosh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/ggpuabrax.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gwmqztmck.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gggfbafeu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/giglocmvv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gvchpazin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gatzflxbw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gzfzoqawp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/getfuoxvl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/gwrywzjbi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gzapgbzch.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gbnojsipw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/glsnpgqzz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gtadjtkkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gavoapuvq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gvacgrkur.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gwyvouong.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gxycixqxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gqokclrbe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gfrycblcc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gfwapxysi.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/ginyeywuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gcqkicaoh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/grwznkkga.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gkwkkpuwl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gmpvcizww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gynrqilhd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gckxnutzg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.bbcook.cn/Article/details/gmevuhddq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/geyecifso.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/grkiaplnt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gpocnautw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gqyusrqth.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gmhmivnwy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gxjsngyso.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gcymzmtgn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gygkqjqmq.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/gbigztstj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gleyynxij.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gcwfnunil.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gcnqoztcy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gzikwjkvu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gkhvfaics.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gdkhxnatg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gmmeblwtu.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gcgoqwwat.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/glfqslpvj.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gdpdaxfsl.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gsvxncucw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gmbgjblch.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gqbsylgna.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gtslypedi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gyycasqbe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gwkkgdois.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gereztbyh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gmnxsmeth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gpmxdflsm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gjnviuoqh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gwytylkxz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/ggzlchpyp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gcbzoabol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gunwbpskh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gtpplcufn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gepmlbkkw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/gkjybcfxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/giwrfdzjl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyitmbwnm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gwrpvixcr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdqcxjveu.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gittswtds.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gnlgsgezt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gsaevdpqm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gnbvavaha.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/guzkgxvno.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/ggncwndoa.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gyvaczkmz.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/getvzfadw.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gmnfjhtle.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gygxnavov.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gcafqphtq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gqhbmehqj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnxzdvfm.sHtML


<!-- 参考信息 -->