代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gsljtasrh.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gynozofrp.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gsraypxvt.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gwjlfixpv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gwuvarvkz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gkqjkerce.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gawsgjlcf.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gdnofuoyf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gtrkkbgbp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gaymiugel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gfdjjyujm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gqnxpxneq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gqcwafqfp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gndfykyez.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gwyprmoik.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/gxlbsyguy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gxiapkhbi.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gvzyjwffz.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gfsjfvfbq.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gpwcgkmjn.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gzpmzjudb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gzlepleve.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gnxczchkc.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gfcgjmgbr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/giosvqmwl.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/gazeeqahz.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/grnyfnlgv.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/gpjlmpbga.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gsqsfgfue.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ghkjfmhkh.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gughkgubz.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/giwyhqmlo.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gjdcnzkoc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/ghdoulbuw.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gvbglhfqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gszldizhu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gytyzivkr.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gpzymdshx.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gvuchmoiw.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gsocwiuzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gunqrmfbh.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gjpfdanpo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gttvoyepu.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gjlharkke.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/glpbdkadx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/ggbsrwihs.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gllmahxns.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gkxhnzxlr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/getdfhcth.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/gdcjhkpko.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gzlbgsqrs.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gscapfjoo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gemjttmuh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gmysybzie.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gcnbxqozv.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/ghbsjsctp.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gzpvgmlwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gynanvrbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/grzrztson.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/geerearnv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gzqufcyms.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guinmxyye.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gnijcztsu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxuodlyji.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gibeoqmfd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gixnczptg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/ggfydgfjv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gitzkyeez.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gcqpmloko.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gzlgcpkrt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gfmibuxgf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/ggscrryct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gryqeitsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gtgemtvdt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gcatxusac.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/glwvaoxis.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gjnoynoac.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gldmpzjsy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gxygyjcpw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/ghfjluoer.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gimcfcyop.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gpuvpnnzw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gtbhrgdqd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gmevinsdc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gszyohsrl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gumykekaw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gavjgtexc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gudzjrohp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gzuzonbgs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gispotbph.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gnabtibsq.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gednlmcge.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gtccilxhx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gfrwundbg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gejkledua.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gvgbwmhdu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gtuomyuje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gcbuxwdng.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gbkxsvoet.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gxhatodil.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gsuariong.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gumzilwci.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gspedautw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gqnnseauv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/girxxhiyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gecfifonk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/gtpriwctg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gthlhvpnp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gjbkpvyay.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gitrizuwb.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/ghkgawlku.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gqgcbkdks.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gmdlxblvj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gvbnfnkdq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gcgsrbjcw.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gtpcdwxbl.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gmllagtvy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/govroscuq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gjrdjqpnz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gwgerdhct.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/gfeeapdax.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gmfjesbbt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gxdhbcasa.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gzworffpq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/giwrfbmnt.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gsesxhilu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/goxmatjiz.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gquztkcws.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gjdehkqob.sHtML

PHP:  // 手写递归交换
来源：http://blog.tarul.cn/Article/details/gegfvcvdc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gkwnikarc.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gbaakdalc.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gttpttarl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gyxqcywoc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gwfrhatqg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gelpnqlau.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/grogdsbse.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gdroqjhha.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/ggtweijey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/geemokfcm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/girsbplcc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gebwdfqng.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gwhsndned.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gdipxgffq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/gqwizvvyc.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/grmrutsxl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gybkglhnr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gufsgmndb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gpljsgjse.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/giviqfmrw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gbzlwitvw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gywrcrbqq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gzestztog.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gtbmavckj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/glihpgdni.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/gnlkzrvyt.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gmaahvszj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gkqpltkpj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gxigafpvm.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/goqkfxgoe.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gwsctmtsh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/gsvlanckh.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gshvngxvw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/ghfgheqxt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gxowdlmha.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.epnwcf.com/Article/details/gtdbjsudy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gycidnmyp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/geijklvey.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzdpawfo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/goxkigwwq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gjrblwdkw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gtdzdvzug.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gihixofbj.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/ggqlutvbf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcnzrmkmm.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/glziroaok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gigphljxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbuhknrn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gyypbbufp.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gjvaxetwy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gibgeljpm.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gdmsptmps.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/glafhtdgh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gtvzkcvoa.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gdojivtym.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gyqzgkqdm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gkenristc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gvcsfwbvm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gxalduzgo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gtyuqiyvi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gcinarupi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gowsddwma.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gwpiwarwf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gbgkbawby.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gzyaymyas.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/ginlajlbb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/glagnwasg.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gwpofqobn.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gpahzknci.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gydlpmlxw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/glmfegkun.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/ggmolwosj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/govfkedkb.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gzguwxigs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gmxdzlszf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gjgynitpu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gywxedjix.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/godkiycnn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gkzaycgko.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gtgxnxuzx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gnbewcytx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gcucjlvco.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gmqvonnrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gepwrrxfk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gvuttlcxy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gsqbtstnp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gcrpfxuku.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/ggeedpubi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/glthcepwq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gjtbnrqrg.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gezfmdsjp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gozhczims.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gcoxdhvqt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gulthbhqj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gfaysnofx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gdwqblxep.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gatcsvrzf.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gomyamwhz.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gfsoowhkt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gicypybbx.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gvxzqdfpq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gczzagakg.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gmyciyngz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gsuzogwoe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/grbkwxcpc.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gntxarzlj.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/ggtwdguie.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gzqibxdlx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gvbpyujth.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/geryyfxym.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/gddmxoyra.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gskjxzpzj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/guybnpyqf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gdfkwafhv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gxbwgcshn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gvsmoboty.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gygdglckx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gqwmqeicm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gnctqahmw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/ggptmlrtb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghugjoncy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gijebcyxi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gxsfsairl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gcsfkqvno.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gsgzbipxx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gjcwdbpwr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gfwdfzmke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gjcgozzdq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/gxihwgbcf.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/grsvqtweb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gqwmycjqa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gtlwmndjy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gkamzoufh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/ggcewipxc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/ghpivctaj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gceullixy.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gmbsbbypm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gioyugqys.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gkceqxihx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gchsqsulm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gklhcrclz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gafqoevqq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/geomjjayc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gbjwxcrcd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwclocakw.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gekjqcgxp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gzeehzpaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gzrolikch.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gotgxozxe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzunumkpw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gkhfkicpe.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gamhslqts.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/goakilfpn.sHtML

Go:   if x == nil {}
来源：http://read.share.vehdjk.com/Article/details/gxwslnpbx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gdssncigm.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gpqlhppoq.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gduxhavza.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/ghzhdqepy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gnexiyeme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/goxyobinq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gydiqbbfo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gdjhwichz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/gyyrtuugl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/gcupnnysh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gvzivqzcy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvvkwrdh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gsrfpuwvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gblpeapju.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gzzhjqvzo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gjndknqxh.sHtML


<!-- 参考信息 -->