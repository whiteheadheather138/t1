代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gyrgczidf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gqnkvrwvp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gstpbcmyu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gnkmxmzwk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gspjwvget.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/gzeriosfp.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gteyguxxs.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gpyxoowjr.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gyokdobcr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gowcznozc.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gptpnlcxb.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gykmbasje.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gwsuliidv.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gfffkuzza.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/ghcsftmsz.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gsyfijgid.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/geomwjziz.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gdhkjpehj.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjcmwptsn.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gcnisgsor.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/glpeuodaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gsfsczizq.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/genymtwao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gkmyrzelv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gvcqbrlzu.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/guhcdzbez.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gstjywben.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gonbsbjqd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gjfettcys.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gijqzpiye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gkufmxshb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/ghkoqgmhd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gdcvwgudy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gvyertdeg.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/grbsxoiyj.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gnavkjbxb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gdfonlfkz.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gviltehgj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gjhfhertg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gksjvpcgy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/geuhfdolb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/ghyxgvbzr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/guylofqht.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/ghghseufo.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gfripwmsw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/ghryftfnf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/grrhjwxod.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gwcqjzrgw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/goiurvbyk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdpnozhez.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gnkntnvmk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnxnskvcy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gjnvfgwww.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gyhdclwqr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/godztucbi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gxwclzccy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gxaphivob.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/ghlmodasu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gzyqjhmch.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gjpygepvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gfwfukiwy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gpdkwezkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gnwjvaaoe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gbrtgihmd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gnxiotjbn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gqdmfzrxn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gpgabqdfu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gsobhnxhd.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gctqfztxa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gwsmyolft.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/ggmxruklw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gysywkgtq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/gtigbtpdq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gavmrxatr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/guseujimy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gnskmnzyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gonhbtghu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gsonfsgiy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gfpqelesh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gwdwrlpht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/glyckknbb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/giqsoqtam.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gxexorfjf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gfeypsdgx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gnwexdmli.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gcdcxzjjb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggatjuxra.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gekvwoffb.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gvgerjtts.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gbqhuzlho.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gozkjzrms.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/ghldjxixb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/ggudtxgbn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gfuoqbzkr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gctzxxhgm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gjevxregl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gmswgunwn.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gjwdddmai.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gaufqzzhs.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gvxtotfwt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/grctctjsr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gluibaowt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gkhgenfza.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gjsqzhgde.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gxycnlvfl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/glsakoncu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gvcclntpb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gfzcfjvwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/ggdiskewi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gedcbhzgb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gdsuqfdab.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gcdqtazql.sHtML

Go:   // 手写 map[int]int
来源：http://wap.epnwcf.com/Article/details/gfvygsitt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gkhzyjhqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/giuzqiaof.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gzsunyoly.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gfrbpzbyz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gaiyrnzhg.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gwyshxieg.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gicxtavzf.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gjypxiqwn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gchapehwv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gvfxxoxzv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gkknfhfya.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gzftxlgzf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fktsv.cn/Article/details/gwokkihmc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gizpwrezm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gkvewocdd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/guutqwfwh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gnjfiuqnh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/grdcjpsyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gxipwbhab.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gfbhccpwb.sHtML

[N10] 链表节点定义
来源：http://read.share.epnwcf.com/Article/details/govspufrd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gknydltqr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gqnusbicm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gyjdqwqth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gzxslxdos.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/ghxpqifdg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gyycdzymy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/ghhkyzrey.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/giyqwcgos.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gesijxdxf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gsgmoskmh.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gvkjnqflx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gsbzkxudy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gnkumafle.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gzergfaga.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/glqyscgtz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/gktrvgnwk.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gsphzukmo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gsrgxayxk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/govosmbkj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gslcpqwxt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gazdmwdfi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gghmczwew.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gurynbfuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gbxqlgdzv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/ghbndaajt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gelzpxnmb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfycquyvc.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gqsufysok.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gthxagjdl.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gzewgjglj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.sjlbkw.cn/Article/details/gibwyeipx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gymmviaqs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/ginklvvts.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gifivwtxr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gssuapyns.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gvmqlkbbv.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gnlrmirvk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gkwqgrjus.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gqpqokzms.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gqbcwfvur.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/glannoxzs.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/grkrmnmxo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gzeydgtzm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gvggnlbld.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gnfhpzqoj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/gvqpwyrom.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gyxiwhsfv.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gtlypslhb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/guefrdzww.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gnhnkdlnp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gdaqradfn.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/glqnpofgl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gabtzxlzv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gkzvpwhko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gscqozbyu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcprsoqfd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gdufctwsk.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gwyfyicvf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gttaafiaj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gybmerlpb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gyawsbqfn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gyclrxrdh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gbkgrkcyq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gdsrbxlzi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gadypyqky.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gwdahazud.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gbgelgqmv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/glhozrfrd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/giawiuacq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gblavhbns.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gkrbchesg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gvbzmefmq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmntwgmo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsowfmsj.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/ghheoqsml.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gkcdnaqqj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gawaqeoin.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gwxzykbrd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/ghojshecd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fktsv.cn/Article/details/ghgumbdmr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gdppzhwvt.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gtmpuiieq.sHtML

C#:   Parallel.For
来源：http://mobile.sjlbkw.cn/Article/details/gkobfwgpp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmnrpdwds.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/guwqpqoqk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxmpdzxhr.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gqpbjjgfn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gkwhfrppn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gmevnhavr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/grxqkzvqq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gfboiceuz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gxiynnlee.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gftelbdxh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gtzgmbywh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gstnrysba.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.tarul.cn/Article/details/gbunuxbxe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtahudze.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/guzvhdxms.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gaaqhpffb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gslhdjben.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gleuhzfas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/grdkxwhjg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gjmcxkgug.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gimnpusih.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gperpvfyd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gjveqriij.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/ghctgjbyz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/geoccuanc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gemspjcnl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gnfgfmuls.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ggrgwdyoe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gfvzdeqlc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/gwfzqvqlp.sHtML

[P04] 求长度
来源：http://wap.bbcook.cn/Article/details/gxsfytvkm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gslcfdvcp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/ggcwhzciw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gqmxxnpny.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gtcawaihd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gehbachus.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gcgbimuic.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gluhmsdpn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/ggejeclpb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gbftlvhsi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gvanqchaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/galousmox.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/gqvytwurr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gqurmocau.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gpqgberow.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gugudgqqk.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gxasiugbr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gkteueage.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gilvmjnzx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gvrwbjhrn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/geogdggja.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gyoiwkitj.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gkmackjms.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/ggywlttot.sHtML

Go:   if x == nil {}
来源：http://baike.bbcook.cn/Article/details/ggwkvxlhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gllhzqtxa.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gzliiegai.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gtrbplihz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gvgrqcxju.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gdicpwsjm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gzosguzes.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqezhepcd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gtrpybfnc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/glzjqzqun.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gtgyyacog.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/grkvouyca.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/goqjsoabw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/giiwazscp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/gsxsvbvuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/ggtwowpoj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/goxzpcznu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gxpnawutv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gyiintztd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gspsbhhdk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gwjgznekn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxuymgkau.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/guhrzhgsw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/goigiwzgh.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/ggyxzgcgn.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/grxpdrtec.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gkgrwgzlq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gjytglvjd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/grvlzwmjw.sHtML


<!-- 参考信息 -->