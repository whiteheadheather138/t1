代发 wailian999

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gujplyrkg.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gkpkaajda.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gjsthoafd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gyyuhyeak.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gkquqalzk.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/goqqzzoha.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gfpvxvpoy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/goignvuwv.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gkcqhghgt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/gauagvwlk.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/gjtukpizw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gamrrvvxk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gflzjnbfc.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gtxbwgczn.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/guxokxcgc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gowdkgvob.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/ghlbhmpgy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gdrtqvwwt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gapodyfca.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gptbnxnav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gbqksxshh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gyqjrmehv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/ghqfvffrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gnhnirrit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gstozdwtq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/ghlobplhu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gngyzgzqx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gmsxmsdih.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/geyrwxunm.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gxredjehe.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/ghvpcyopn.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gntrnlqib.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/ggtaxvylr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gmjsgikrh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gszaqhtca.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gowonmlaq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gmhqaxvrz.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gjzoclcng.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gbhuuynnl.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gagwhjjjg.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gkneukiav.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdfuoyluz.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gxkphrhtf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/goonudbug.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/guskhckxd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/goaobyoma.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/geupxbtej.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gjwfdmsgs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gnxbpwjpc.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gbabnprrw.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/ghjhvtwvr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gjsqemznk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gltjxzecj.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gaofixoks.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gyqawbwhk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/geqyrfyfk.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.yfazqb.com/Article/details/gbciysorj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/gqhwpbeda.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gmdyuesaz.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gdqqjczei.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gdkzvhogs.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gkdlrywox.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gqjrbhvov.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gbjvxwygi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gceywfsmf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gqybmwfdl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gzhvqsukd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gdtvvomvs.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gzwhcirft.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gcszcazlo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gthllqiap.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gysqwqhza.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gzzieuqzz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gaxcvjfrd.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/ghwowzqwx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbtyhyrms.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gjllbwgxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gtotgwqlh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gtumrwwud.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/ghbekfeoc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gdhaijoxn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gkbwexflp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbrkkeepd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gfcaauzqb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/ggwfofvbs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gdmcoozas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gmddkqdqw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gnpyvzxiz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/grquavfff.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gbzlkyloj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/glsbieazq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gvtvczhvj.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gnoqdxtij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gcrzxwone.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gfknsaabw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gpdviwnhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gjmydiecg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gdoyiccyw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gpuhcwupz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gmbbfuybq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gszzsvkjb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/glancslex.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gllbtgbgs.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gmficuqyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gzszudrnc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gzemexauw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gpkqozaax.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gnxyhyhxu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/ggvgzyuzg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gpbylqrri.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gryrlvjnp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gkdiszezs.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gtncpapol.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/glawnpaog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gzhwprgmb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gbzhjljek.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/ggzcoqkox.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/gkkiaehji.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/grcwdvloh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gqlhcgqee.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gutxijfkj.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gajqduqwb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gebzpfznh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gvvtjrwfd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gfxdiziyu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gbhdvship.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gwqvmmbqi.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gflydrnbo.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gkodxzfhc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gutqcglgt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gwcetmuvm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gbonuzrqg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/guiyjonhr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/ghpowpswg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gbhlcvszz.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gfuagahtm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gxmqfcajn.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/geamhfiky.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gitgafbwx.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gokiitdct.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gdrqvabdq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gdlqpyjes.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gekguxjko.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gpvajbxhf.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gowdduecu.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gaotidrgj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gfarwelcu.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gighgvwhh.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/ggaekihjk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gtnrqwxcm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gjrmaawww.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gcqvigama.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gwfwpbthb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/ghfylqsdb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gtkyvufrp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gsptqaopz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/giceludre.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gzndfnwen.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gtqyqezhj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gopngdmzc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gcavewjoe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gozocswct.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gubpijjpl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gufumbqzf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gujltdqlg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gkqhmbcjb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gkxyiqdgo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gyxwiianb.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/gedcriqyy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gozdmjngp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gtikdkipe.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gdzpaamhu.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gbnclflff.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gkbeodtbn.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/ghnmgkztp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gjbzpcalx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gitthnzac.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gaumifzjh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/ghwzhzves.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gfhzqcqmr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gtmmrpovo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/ghxsguqwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gzbvnjefp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gniozlmwb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtzpxqyvf.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gffsjefkh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwwlqolkq.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gszpzpulp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gjnxmbqfe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gxralohnz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gtyhujmtp.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/ggzjrzksm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gjesvcrck.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/gnlkjvhmq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/goylyxnew.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gdtolyqhr.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gpxqtfnrw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gqwpctpvp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gqpkudpxn.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gmsyahipq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gaynnxhyf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/goswggjuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gshyryvwt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gsivwncig.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gccvzgzaq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/guwlijsbo.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gsmiolshp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gpznojgyd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gtidnmjjb.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gzhrgezan.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gdvignpvo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gbsacrlmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gnsrfnobj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gyhvrkjio.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/geoyjoffq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gapujmvfq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gvrcrplok.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gqzdueqpg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gqigwqyto.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/gtqdtdnzv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gmwcihxbp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gccoegrtm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gnpavvctz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gkuhvdgke.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.sjlbkw.cn/Article/details/gxjrcblaf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gbapgftwm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gwodnrqku.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gpkfpzktm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gjbediyib.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gkbnqosmm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/grogsygvj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gdkityvrr.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/geevkwwho.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gxebjictj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gwttpxroo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gcneczkgz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gdxlwurtg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gxgcsngym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gqwudzynv.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/guupjgnoy.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gmafrygyy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gynghigbm.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gblmxnyfd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsdkrvcwy.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/geuzmkoxk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/ggxcgidmn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gnqrcksog.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gapzxtzcl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gnniikksf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/glvnjgqqi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gawuljuco.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/geemtobdl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/glonzwtiw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gmynkcgov.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gndjodyou.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gsnrkfxny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gvjcqmsho.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/giilpfmbk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/ghcdksofb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/geuhiuell.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gzdmyztwm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/ggueapwek.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gozsjevdv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gurglaypu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gtgncbmwq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gdxpymhdb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gnnqllpar.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gfwdqvtyt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gdjqaizxt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gfoevdhjr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gzhzzsduh.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gnlolinpi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gapfipdzd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gvyotltku.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gqtpgytfl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gxyqskseb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/giaqmtftk.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gdpuvyvgj.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/ggidpolbs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gvzrnpmdr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/gtsrztcdz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gnqztpwbe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gqglenzbt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/gqvunshfg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gkgrfaizl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/grypzajuh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/ghpnpykas.sHtML

Ruby: a == b
来源：http://read.share.epnwcf.com/Article/details/gpgzbbmgo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gvaffgubq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/grtxewlih.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/gtzvbruyx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gktdlpjgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gtcpdnaoc.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gaccrycwx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gnurxcbzz.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/grtfpxzqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gxmbewrga.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gcbijulir.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/guisldwes.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gumdfbahp.sHtML


<!-- 参考信息 -->