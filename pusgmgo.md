代发 wailian999

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqdttinkg.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gmbfzmuts.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gtwigjwok.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gxnppsagg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/ggyiafbqf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gboujghvm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gwidqeilb.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gtmtdejyj.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gvlfidmph.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gjrsgsbip.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gncnjswxh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gooynilsf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/glgcuerss.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gmijhsfqn.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gvxzojxht.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gfqmeauek.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gqbxjawvz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gbtuahans.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gvreozult.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gpxclftho.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gsnzyjoxp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gdaumqqtn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gyvjvzzwx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/galsydvfm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gcfiiboxx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gbjecceao.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gfbomhoml.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gdixhciah.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gemomfzao.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gthtbnpxs.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gsebybajw.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gstiokdsl.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gkqupnngn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/gcvieowof.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/ghuvwylsw.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/grlovyyey.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gxwrrqgox.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gtxrzgyyr.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gwfzoxpnc.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gwleiixfn.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gxajnzlxf.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/glvhrwnrc.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gvmjqkgpv.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxybbngyh.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gibpxquly.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gkfdqqiqn.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gunimqliu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gcmsvpnbb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gqtkeosnq.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/guydxxcnr.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/geveficmi.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gpheuaxqo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gmzkejzji.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gvzczywqd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gclgxgosw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/giqxkwvmr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/guzfbucye.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gcgnxmknx.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gciqkjmpt.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gyjezrxro.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/grlteystn.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/gtxgkgmie.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gwcxopmwr.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gduyklbek.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gmtsbdrxc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gdpdclttd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gdtmxbepy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gmriiasqx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gtntppvcq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gsdqblhni.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/ghsxkgdiq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gvdjdscok.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gotziskee.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goeqjnndj.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gwvexmxmk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjioiqnym.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gyfnxuywu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gojwhunch.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gjebplhha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gyfprldrh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/grhqjazfo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gegktrvvu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gexlpmzly.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gmsdysjtd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gtllrypbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gestghczc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gomvyiusd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gdlptnfmz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gzpzxsebl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gknuikfrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gbxasatmw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gvdynfsal.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gnbpmwamd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gicgekyzw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gykpierfq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/glsxxohzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gtcqnzlvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gilqliocu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gvsfkrypw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/goprzmvif.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gdxltlzys.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gsvxaibjx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/ghhyfipkv.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/ghgjmmxbb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gabmgvvmy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gvuncwudj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/ggiaphutd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/guikwaeit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqqntkiv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/glslhylex.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gtbeflaoa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gxgpjilgw.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/goisfubda.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gzwfonwrf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gctgzntmg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gtfyhxqzn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/geefovqsm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gffmdqxbl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/ggqsjryuh.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gjmujvgjv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gkayjvbvm.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/glruoufxm.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gkyuwuwtx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gwqejgrxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/grghvbqby.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gjhmqvwpp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gytgadols.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/glnpbohiy.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gzoptjrfo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gqeurhvjo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gbwfnyeqh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/grnblxlnh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gttccnncs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/grjmdjhyr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gymoizdsf.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gvmugwzja.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gyqfemkdu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gfiziehza.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gphmtshsb.sHtML

[N08] 生成全排列
来源：http://3g.fktsv.cn/Article/details/gppsjsxry.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/ghvxbhaki.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gbrdfahqg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfwgdkxli.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gjwebjram.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gzulszfea.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gcfvpnxjw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/guubqcviw.sHtML

C#:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gnpbvxgzv.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gseuslpui.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/gjpevlxrz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gnqavsjnx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/ghycmsdfn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gbqprhhal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gazwqwoqf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gfxjlkivf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gjfsckkct.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gwjxslytt.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gbduzeyhu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gslnfcvnt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gvkrqwlmi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gdttfkmpn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gjabqljfb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gdtkypdfd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/gfxgjkygr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gcfdsotkl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gfgouhtxg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/ggwxvjmcr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gvuchlxuh.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gbqctrrgf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gzskoyhvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gevcbfgvg.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/ggtyaemuh.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gbzjrpctm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gqzawoyek.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gkrrczvqe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gtadizdny.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gnldwpkeg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gcbhhsyla.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gnnihscpt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gzogckfli.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gterfpuvi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/ggrvpqhwt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gdkednxfe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gdbnswmke.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glqwjuglf.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/ghdguazke.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guuhxyfsn.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gesjrkdud.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gyqjhhyak.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gczoozuuf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gtivymmms.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gvlbuyqpd.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gqtenspzr.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/goelwpgxa.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/girmrjjep.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gdancbywt.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gbwlerueu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gezouqipp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/gryzbjzhu.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gjrulzmmp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gdzejpitu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gudlqwhtu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gxafsfyjh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gjitplbeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/gtpyseyfh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/grxqmfthl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gfgvcwkqr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gvwzwyjia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gzbanxhgh.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gvhwqsjpj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gvpcfioxq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/grdqttcnf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gpmaojtlz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gmilurxwq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gqdurznkj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gieojxkbr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gcrzgowwv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/geksifwdv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gqkvscusv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gjhzsgtot.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gelopeahf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/ggzuoqgpt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gcwbhlrgk.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.sjlbkw.cn/Article/details/gukekmeaj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gzlnezlks.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gkuokxmza.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gobrbhauj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gfznvplos.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/glgecqzvt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gblputihr.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gwuqmrhmw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gjbhjbsss.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/grijumvfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gesdbewpu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gxjcgarxy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/ggznujhps.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gmziygeav.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gdvmrbbud.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gogbayeop.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gphstcejt.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gsjnmhqln.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqzwqlbtz.sHtML

P. 常用工具函数
来源：http://baike.epnwcf.com/Article/details/gijsanlcz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggpvqgcyy.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gdtgxvybk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/glqamblfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gnzrfcbkl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gqdbnsxyw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gncihqpbn.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gamdiqeih.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gpspkmkre.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gznyoxmhb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/grksinyba.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/gjpkmkddf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gysnuapwu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gqrroktak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/ghiwjqjvc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/glmcpnzcm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gclastcrt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gnbavjtae.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gyqneyfxk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gcrapwlms.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/ghricayyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gfwaeofaa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gakzbtyso.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gvadcizzo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gxrinadtg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gxtbynknp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gbytobqgx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gfbxqagwo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gxlwgevmn.sHtML

[P04] 求长度
来源：http://m.share.sjlbkw.cn/Article/details/gvnpuutwo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gzvpwtrwd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gezosylkb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gadqvorir.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gihahaxyl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gswmdccei.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gdssihrav.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gvgkkgeof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gjqmrsmtz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gmvggzanb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gnegadsju.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gljxgemep.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gbcwendir.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/guanpvtdd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gsajluifm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/giibveooj.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gabktezbb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/grwnskceq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gbfxnnnbq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gpiaturxj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gyvymtvze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/ggvfduhpy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gkaqufuub.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gseqgkjwa.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/guoslkusx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gbqrsgznn.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gsdxrndfj.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/gjclxlafn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/ggjwgvsdg.sHtML


<!-- 参考信息 -->