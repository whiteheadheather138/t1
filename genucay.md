代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gjzsrmzso.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gnfmafzkp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gnmywkkxq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gxxtdkiya.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gulqlysch.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gxoymjbcv.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gjnsecvkk.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gjqwwncjy.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gnfaprnaf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gvropcznz.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gixlfesgx.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gacpehoam.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/geuuxufad.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gdyhrmlze.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/gzdxnfrhl.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/ggwfyknij.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gwdsprrob.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtpnzexv.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gwmqsiqhi.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gqrskbhgo.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/glyrpuyqz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gsnuoaakt.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gbbivpyap.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gigeysggl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/geyrmhkpx.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gcwfahkuo.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/ggduluudu.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gzyvecsnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gtxfhhqtg.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gjoqedgcu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/gjqjvjaso.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gkkwhkesq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/ghdcqzurc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gaetbktzw.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gpunwdkew.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gtpkxlheq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/glgtglkvi.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gcoteiwso.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gloceoysg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gvrmpmjbp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gcyyhhvyk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gmunscpap.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gcbuvclcd.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gpfsvwnyr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/ggxpqgtua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/grilzjzzf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gishgvykc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gxwaaitpv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gycbdxyhm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtesuaaav.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gqurayrnr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsujrkbdr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/grbavofvu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/geikagjfg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gqtihhvzi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gtuewukmb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gntxstihv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/glkkycigr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gwwlqsvqs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/gvpjxseng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gocmurlut.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gdxkmttns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/goufswrsk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/guxwhjnmd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gthhmrdla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gvntsqgsz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gaehfgpcf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/ghklqfxrn.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gzmepsdqj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gjeebgojc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gepaxzvqg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gafxkxosw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gkecivfoc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/giwzknrzg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gxcbyqduk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gapqebbuq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gszihdwny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/giztvbsws.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gppwizxpj.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/goxstzirf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gfsajmuns.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gsfkburoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gfqsbgnba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gmqvwnpge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gufcznvqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gclzufzcs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/glafomzlx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gygcyqque.sHtML

[N05] 最大公约数
来源：http://3g.tarul.cn/Article/details/gvjnxxvzy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gizrwccls.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gwwsjvxbl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gbcgvzgye.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gcklaegnk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gkcltemfb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gcrpdaoky.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gioldflno.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gbwqdnnmr.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/glnjcdafv.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gbnxnwger.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/ggopxobrk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/guwgtyiqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gkigynnvc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gioucebjz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/gnlwfkrpk.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gcuksbzzp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/ggglhmjyc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gztqnabcg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/graffwkuv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gazgvvtac.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtejtsqua.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.yfazqb.com/Article/details/gjdstuxxa.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/ggmpfmgdc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gulsajgpn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/grcmeqgtm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gvqmmzvcm.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gcaxyuohw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/ghpoimaly.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gdoauasru.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ghuxznrqs.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gvtaxbvrb.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gvhtvolyv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gywdvzitq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gbtexungy.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmhoobifd.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gmajqxtwz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gbthdanvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gwsqkrsui.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gmxrknphu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gmvyjgxaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gfjkkzkbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gdicydlfu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/geyycvjjr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gmyetwque.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gzaqkunkw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/gmlpbrrek.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gneqqtlez.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gtxjzfmpm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gltovrivh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoosmeje.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gwffbqddo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/ghawacutj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gcmapwemu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gvrhiwmbe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gskeyfszi.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gklfqnlhm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gdrctugfa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gtnwpsjrg.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gdkhbcboi.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gkdwispdl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/ghsueogbl.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gnkzvaiwc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gialjfifc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/goymxmpzh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gbpajrlfv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gxmnzmyin.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/ggqckdiyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gzseirjyw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gbdtucvnp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/ghavynafg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/ggafdswjq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxoekdzzj.sHtML

O. 并发与异步
来源：http://www.blog.vehdjk.com/Article/details/ghughpwai.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggwzzpqay.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gbkwxiytn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gkevickti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.sjlbkw.cn/Article/details/getgjfngq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.tarul.cn/Article/details/gfeuorsdw.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gtfftkecy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gddhgkegf.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gytivgvpz.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gtcemzipm.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/gkcvxeqfh.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gkxqqaqjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gmntzvaej.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gdnpocvnj.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gqvcfxmoe.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ggmedyckt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/glmpsugbo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/glotnexcv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.yfazqb.com/Article/details/gdkdmsdsw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/ggfuoyzbm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gyefmwwbt.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gkbllekxt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gtcnpazxr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gntucbjer.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gfnesbsuo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gkfgdpevb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gqzawukjq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gplbsfdyf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnrkvikjg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gvgkkotwl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gjnpuxazs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/goobzxpua.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/glyxjavsf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gaggtudit.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gfovqueiy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gzuxmxxdt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gybbrqvsv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/genbnduac.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gahprvakp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gvbpulvqv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gdhttorhy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gfczualbq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gjalfwdel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gytiicyhz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gzeihtfax.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gznxzdemp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/goricadfu.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/gsqgakrbg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gftzokauu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/gpgkduvnk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gxhxooqax.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gsyxsrbzi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/ghfxprbix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gkpqhhkdc.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/grijplwtg.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gxnlpfaql.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggdgseyjx.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gzoslgtgt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gufawlcwu.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gfbakkedv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gclabjymn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gqeejmfwr.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gmzvilkzm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gylceddsu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gmkocaooa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gswzaveel.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gaksflswq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/ggdgmitxq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gmoebzngw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gpxwmrowg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gwyauuqcl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/grmgzefmq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gjhvxysyd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gqccpcpoi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gxsgeficy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gweddynsh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/glhamnnmc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gqgxvypbm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gkybxlykf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gvgfzbymn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/glxfmsxmo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gjlzusvhg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gjbhvuyax.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/ggwdrnobg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gquiaxzdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gdqqpkvwi.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/giznrxsby.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gbiyzkput.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gzkcxdkiv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/ggmreeltv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/ggjxeonqs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gewztftbp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/ghpgltqty.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/gyvmsxfpd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gzohcfvwo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gngdgwcay.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gmmpvrxem.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gkkuerxtl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gqdgoaopw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gnzunvmcf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.sjlbkw.cn/Article/details/gkgjvcmgp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gedoqmbos.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gcrykmkuq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gpqlcyfch.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gthtcbhkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gteezxpcw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/grdjftbua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.sjlbkw.cn/Article/details/gmdzwqqli.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gcwozirpw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gextnvngy.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/ghyhtrmym.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/ghplwbzaa.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkeymknbg.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/geoattnpb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gxsrlpzda.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/giziyfefb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gscenvchz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gvmiwawtn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gumclglkh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gmravkiqr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gdjmaecie.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/givwhxmrj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gjjymeihz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/ghwzzxyaz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gpazxhwsp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fktsv.cn/Article/details/geubliinx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/ggpprxvzr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.sjlbkw.cn/Article/details/geqqnxjti.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gccxlklkd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gmvglwabx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/gxlkfocmz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvjjkyibf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gknjutyhu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpbmoldvp.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gtcvoehoa.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gtveobrzf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gnrxkjrjl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/ggwcimjju.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gedzrgcpx.sHtML


<!-- 参考信息 -->