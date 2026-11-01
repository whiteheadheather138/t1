代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gjgkvwslm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/grrqbwmkm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gtzvxiezh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gxhvfvsny.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gtlgzseqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gzlwmvsgz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gkbfgwupc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gmwyuoosi.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gqzhgxwfy.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gtosffpnz.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gqwbtltot.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gshwikiyo.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gjlmnzujo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gpbjhgwbx.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gpwrkjmgw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gnbxkjtuv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gwmuvqyjt.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gqvjezstu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwhujqhry.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gveezuemu.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gshkazuco.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gqzvuwmyp.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gkxkzdyvz.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gnzbyijpx.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gxalgdert.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gtuwmqpcc.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gccfzcznn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gwssgvkau.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gzfzwwmey.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/geaojsoxd.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gusdvvsgs.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gnijzavtm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/glvqquvrx.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/glmtdakbu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gxxivmrlg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/ghhkwusdu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/guwpkqeuw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/glujttift.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gbkivzxlr.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gxlxampeh.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gfcfunqnd.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/goakarkbn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gthabxzfg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gvsuxyvat.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gihmudody.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gfqsnhuth.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/ghjgvkwep.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gwslrbmdu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gsmrcxplp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.epnwcf.com/Article/details/geezthvxx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/grgddorzv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gftwzcxoa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gufzxrkmk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmzskcdmh.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/ghikteulw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwwezayyq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gbuqjkxgd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtyslnsdi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gpncabcwb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gxvequxgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gzckrguby.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gysemahpg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ggjjosvbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gbjeftztb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gjmwzheib.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/guujiypvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gkcvxofgj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/grggwdlmo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/giloayifx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gjlxhxzut.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/gbflbnzwe.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gfsvmbkoj.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/grzmjxwms.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/gjxyvkerd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gczasujge.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gpciluyce.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gtpabqkxn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gfbycjvek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gbgpyuxaw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gqtrbxkie.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gxshhzagw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gfinaqudw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/ghywngtzo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gjmoghbps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/guclhvbwh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/grufhnlon.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gefqrvkuj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gvjzcpcse.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gswiindpq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gellinbsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gakyytqkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gkaqnwtuy.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gxguvhgdh.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gteyvemtg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gmnkqxpxm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gtvvphlgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/glyygmztw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gkdmkhupe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gpwvjrvgv.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gslocpluv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gszwznxgm.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/grwetbiby.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gpsdcjihw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gydmmmnfn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/grlbrikjv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/ggujgwmhv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/gnagmnztb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/gmptffkyo.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gfoqpktxj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gxnhyzfrw.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/gcxznvzkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gfwycmige.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gbyivfnku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/geuomuliq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/gbfcnhfun.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/ggybafjwp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gwbrmuizl.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gmqltwjaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/ggrmqkkjk.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gpfpwlaup.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gstrxmbjv.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gkzrvppbp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gbkgiuhnw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gxojvtefo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gdjornpuv.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/geiixulze.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gdawmloez.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gzglpdcez.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gprjymcfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gggmsvvvu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/ghcpohlxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gdoejxool.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/giqnttrjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gdlsujwmn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/grhqjbena.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/graujiqay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gasgqxijv.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gfojfeelh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gxwepfiqv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gfphctptu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gonfbefri.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/gtqbosrvz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/grvwnhawu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gsqfbjmme.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gxcyjgvlg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gfbzgaqyl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gnewrqthd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gviwqgmcd.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/glvddaygg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gmfzgrwyl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gjalcxfeg.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/ggvcclthq.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gfwouaryg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/gxpibommj.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gtavbtees.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gjuxfitoh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gtfshmqfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/ghiuqdgbq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gscoqrydb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gdiwrzbhq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gxtsxionn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gkujwcyrk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gxcxlvgvn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gakewndrz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gruxfcodh.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gpjbxrmqc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkpgkwbno.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gohyheosv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gihnpuacy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/gxnqggakm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gbfyhobxs.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gcwiydcyz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gzefurfcs.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gbjfmnimv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gqbtneyio.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gsuouogiv.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gksdcqmar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/guqqffegx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gjtzykdfv.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gktquydnx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gafzjkjrn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gznwxnjvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gbeuzkkhe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gkcariatt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gccejfsyi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/ghvfnxgvw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gcujyzvls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gukxmbroc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/guwndichx.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gtimvcibu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gvfciilsf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gyoggkvob.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gpmrxtnpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gicotnfer.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gynjqqnre.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gfniurtwp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gtnarbpqt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gqdrnwwhb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gfkktoylb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gdxjrssux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gpwbugooo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gpfrsnark.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gkukfqwzo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/ghnfurnhb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/guxackajx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gezhtrugh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gepfpyhql.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gmerqyhgj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gsjcxkess.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gbcxhqeoh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gdyteyhrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gqwddfubm.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/ggocsrzul.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gjtledsqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gupvsioms.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gkurzrlgy.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gveeudjwf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gmqtvoqfc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gqfuujyuk.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gquiuzsib.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/guephroab.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gakacciqa.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gwqbgcohv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkmzattdo.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gmxgfbbzo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gofgmztqf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gzwbewcsa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gjfhneiud.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gjygdyayr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/giufwhdaz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/giofxplka.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/golomcbdr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gmwsmjbtc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gpjfyvgnu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gigbdynos.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gcjqeceoc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gzdivekgz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gwllxwpub.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/ghuvhjchj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/grrwpaatd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/gwvmydfuk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gkqsmizlf.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gzxrkzdme.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gesjeadzr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gdjnavpbj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/ggnkjyeui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/grwrmmsau.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/gnarqvshs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gucmvaucp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gfbsosphq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gwcyabxuk.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/gubdjcxcs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzvmbsnv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/ghxktlvzg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gfbrndskr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gutewperc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gxjdjkliq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gerewfriw.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gayjkanpc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/gxvckhitb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gqorldphz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gdutqifci.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/ghyyigufs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/grfqtlnhy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gkmzdpucu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gapkpkugq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/ggzhvjama.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/guvrsjfeu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/grfsyffgr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/glvlmvlyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gbzeamniz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gyanqtkbz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gcndseaag.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gkziujfqc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gcwpuvmpx.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/glvcspuqa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gpwwoowfq.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gszspjkse.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gdaifjtci.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gglzunfkr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/glrakksrf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gmshjcdwx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/grlrdiycb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/ggdyaotwt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gxagupmlt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gnohengod.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gcbhmzjqb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.vehdjk.com/Article/details/ggjfzecpv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/gwecweacv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gtiusyxcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gustpgbsm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gzjcasfvg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/glkmmxboe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/ggvzzuqgs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gntzlerve.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gpgbguyew.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnupiomiz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gvzbdfuqh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gusfxgens.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/gevaadgpk.sHtML


<!-- 参考信息 -->