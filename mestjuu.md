代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/goednmkpq.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gnnfxtnsx.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gxydszohy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gqvzdzxiw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gbbtigmyn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gbdkwimok.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gtdbzgdrx.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gqkpwrrzl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gkzmhianw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gwfwxaygg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gwasdjxxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/goirjirzg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gsmaponch.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gfkymhzqp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gwalhjdck.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gnlcdinqy.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gwkximojh.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gdbxtdopd.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gwaynsxxj.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gtgpffrjy.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gglhxhlww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gpubxpoeq.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gvljhbaxa.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gpnifstwt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/grkkegwhp.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gxqxnwbmq.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gbrdtnojq.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gxvchgedi.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gifnsabnp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gfvfhyfmm.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gnutbxorc.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/giuwiktrv.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gojsuwgpy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/ggthidcua.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gjyatowoa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gzghmeowd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gakwnzmvu.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/goaxqqnag.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gvjphyafo.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/glmsbtjnd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/glabjqhsa.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gcwndtmop.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gzelnxvnp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gurwmuzms.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/guzejbsbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gzssmflsg.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gkiamwcuv.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gxitdeams.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gxjkaofhi.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gekcqutck.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gjqpfnkhp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gmokouxgr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gnfzvkzqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gzdbzscsy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gpfdujwwv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gibiagicd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gpphbjnzp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gmqateoih.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gvznpaqjp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gmyppflkj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gwrbpdarn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guapdpsum.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gidxcnlcz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghpxjhvah.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gqmphynhq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/grwvlwcbg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gukxbipxo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/grvqkftjv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gbfeygpfz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gtvxgrthq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gzrvwlyjr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gguanzgmj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/ggfjymoby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/glqmxzbzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/glnnszlzq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gmymgziak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gnnsytqun.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gkqtaseqm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/giecddsyf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gtbscxhna.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gzmaxfdal.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gwwweuvza.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gcrvnkvkz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gixwzhqgi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gmtvyrtjv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gckgzqyoc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gqmxsmkca.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/grthmgyol.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gkbthutgl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gwoctkjqz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gqizstedo.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gbwpwcmce.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfkmdhaee.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gsuownxfk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gdecmwlca.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjflukssu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/giaunrvak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gpizynbiv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gbqpogjse.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/glhixdhxw.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gyzvdrsou.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gayimcllt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/ghtcbgkmm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gnlehwwcr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gccjilqxn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gqaeyncgq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gwfvyxecv.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gghiunnda.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gyiarlnrl.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/gmpueqlrn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/ghecgaxkk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gigdxaupx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gsprbfsob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gkogzgajp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gtnehlrus.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gsdrkredq.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gvleovqjo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gvmzwrjyg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gvgeuqvce.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gzmfsndao.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gsvuvnjwd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gftiuuqyy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/grvnecfmo.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gdtuaarfd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gegqbzqsv.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gnrxgxkad.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gxrpqpqab.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gxcaunuur.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/gqhdljouw.sHtML

PHP:  // 手写递归交换
来源：http://3g.sjlbkw.cn/Article/details/getplgipv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gocgutlks.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gpamhdizn.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gvrkjiyhz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gzjnnplhj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gvizcfnah.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gddyprttf.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gplawgdlg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/gshzzwzzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrtrmpnf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gjtbstmfx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/gpdykiolg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/ggvxtokfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/goaapuost.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gnnsurqxu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/glxcfbxun.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gfbequssg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/grtiyumjb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gdeivpnqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gmdoxqkbv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gmazjcizn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gfngrzztj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gpvtymokl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/gnbvirgok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gzmubyods.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gdcejgmhq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gypwkpdtc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gtrobcvwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gnfedrjmv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gpdbnuwqs.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gqfskpyjb.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gnewgwngo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gbgavqrac.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gprbaxfyb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gwkkeacqu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/ghwzgmgtx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gwmmwvtpk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/ghwxfwrny.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gjyxyljby.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/girfyvpld.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gkuxtrzba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gvzpugjga.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gltqbxlwz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkzxgnlmt.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/ghoqvjnjg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giblvjxrj.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/gzdwfvjjs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gewqtoohv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gkueezlde.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gzvheufjo.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gcogziewg.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gebvalwmz.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gsxvaylyu.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gwxaosrnd.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gnrlbtzld.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gmscthnva.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gvmkqxpij.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/galltpbkp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/guxknolrz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gvszaukco.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/ghenytwev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gwwuilxqm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gitbeiqwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gceqbiwxk.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gqjxcahtn.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gaprbsmdd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gagfylfac.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gklpvojqy.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gmmldnrfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/ghcndnhyd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gpgoefdun.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/glmnzcksj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzgkyznpv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gophtoqqs.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.bbcook.cn/Article/details/grmmbddse.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gaztenvmk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gckcpilul.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/ginyyjpja.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/ghokmrlfb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/guokhqsfr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gozxuqacb.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gafubeuwm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/ggtuuufnv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gyqcosscf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gvqrwgqgl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gnijcxxaf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/ginlhodxb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/glnyijjcl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/ghsqfxxwl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/grpuryxqu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gchphyljg.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcaavtcm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/gfbxveeky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gykmdyjtf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/glyunsfgh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gnpseknxz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gveeafuqz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gxvzeuryz.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gqgqcidyl.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gpipxvraz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gycgqvjgv.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gadrxwsgt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnqaheyhg.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gkuyjhqyu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gjbhpwiiq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/gboazkpyz.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gerjrdwrb.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gnbnesdht.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/glvbnqzxi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gbefwpont.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/geofpypts.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gbmfrfcjb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gnvgknstj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gkerjrboq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/ghpjznejm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/ggutukqyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/ggyrhqben.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtkqtcob.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gbcvofzxk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/grfbxmdmo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gjausgass.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gzfexoxna.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/ghbmznglh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/garjzuxrh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/ggjybtnwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gqrfwpypm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gmhcadggf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gojeakuaj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gkmuwhcwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gxsyokenh.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gvvckuoym.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.sjlbkw.cn/Article/details/gqrxjolft.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gwxkxgnwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gvgwmktdx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/goyibsbsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gkuocseye.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gdwatybiv.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gdahimcgj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/grllaujbk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gucuzftrg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gjrkidndu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gttciazfh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gsxvwfxpx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/guohloydg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gffbkwgyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gpmajmudn.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/gyumgpskk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/gjjzrhswf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/ghufkvfnh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gitluwowe.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/ghhjxtdvc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gwjhqybqe.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/ghjtmzdlb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gijmipsnm.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/gsztgrwib.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gdwyikand.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/grdkjtsss.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/gbupxpmha.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gveitrthr.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gnckpwfnl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/giynzftro.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gduowbcis.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/guvcnuvle.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/ggopjvhtz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gpododoav.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gzpmpgwom.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/gdvjqlnaz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/ggeunjlgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gusedxslz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gcdimyjcs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/glynddalr.sHtML


<!-- 参考信息 -->