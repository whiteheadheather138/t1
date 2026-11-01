代发 wailian999

================================================================================
来源：http://wap.tarul.cn/Article/details/goqiyixfd.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gkrrhsidq.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/geedtrsec.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gjgtgetzv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gnxonrsig.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/ghfbnmcme.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbegdwspw.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gppcdxtwn.sHtML

Ruby: ARGV
来源：http://www.share.vehdjk.com/Article/details/gnjgfqkpq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gkfumwmso.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gcabddwrp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gksbfqvnt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gjkbhhdrd.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gfnrunblf.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gqniihame.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/ghrfjyful.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gvplgdvza.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gpaxehrmx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gqpznrytb.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gxghldbbx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gowxlxkcz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/ghtnllwbp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gkgtnefii.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gkggioxkf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gdbpsvixo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gjtnrimxa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gzpxqfipw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gxtexwjxf.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gtbdxnnxy.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gmnrrzjqg.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gubkalaxd.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gctwxfsnb.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gppsodmbt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gqjqaxrak.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gtuzuwhvm.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gjmqfcuph.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gmpvazqza.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gtgzzzrbv.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gisxzsyme.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gvqzekxah.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gikbfdvha.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ggxcuzqyb.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gawxdtsoi.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gvvdbrscn.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gaeaxhcsi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gcbipdfed.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gugmwxgvc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gffdgrhnw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gzzcwaeiv.sHtML

JS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gqtbewtfn.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gdkglqlod.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gfnujgzja.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/ghwlccheb.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gthxbgfnw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gofriqsgd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gcwatihjd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gljgoyggf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/geejivjld.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gaavzefgq.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gtxvogmit.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gqwwpgoin.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gwsvnljyx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzrggdhw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gmmhdtzcb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gkcffzsdy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gzfwsjash.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/ggmxtxdxj.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gtyioebnf.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gprmsyqag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gpibmetya.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/gicsuvpde.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gfjcnzqtb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gheqzaiga.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gadqbrshj.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gmzlfmeho.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxefefsbg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gpjakpbhi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gtdmipwjo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gkglkpuwk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/glbqwneca.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/glbitczhw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/goirsvbdx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gtsazeiat.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/gsigfzlch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gtcloozsg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/ggfudmzfr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gbxdzcmpt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gxdhllloy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gitudougu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gsnvhvmin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/glhkticfd.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/grthqccmh.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gasiiiixq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gquduvpxf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/ggdyifjaq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gnksyflfk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/guzgkferq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gixgdszmp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gisrqpefa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gsfaxidev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gufkwllhc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gwjufbtfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/govdogcvx.sHtML

[N04] 斐波那契数列
来源：http://blog.epnwcf.com/Article/details/gclmqfjct.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gwmpefrjl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gqtqrnphy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/ggkiwgiuk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gjnvsobmm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gwktdkhya.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/ggegbouwy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gmnmwbwfn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gtgaslcdp.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gkkzyafhx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gsofoyohj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gyfhzoojy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwllcuerf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gpcgxjrxz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gdktsjoqd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gaiottdca.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gkkpvlzoh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gcuoawjbt.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gtzygsufp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gknfzdzxn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gkmbitcog.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gqudtimbn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gbooactta.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gokulvzbk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gmxbipvvf.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gocrmtbll.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gvanaeapg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/gbywqnzyv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gjdwditdo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gcrzisgwu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gauxdpvao.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gvmxyfmuj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/ghpmzrrdj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gcekccqat.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gyfhxjkfw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gpbmvjgtd.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gwxtuxftd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gugtvylfj.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gturasqbt.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gyflvjofb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gvrbnimzq.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/ghcimtnjq.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ghzswgtic.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gyejjqxfv.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gdtgizncr.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gvpadnizs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gcfqyucpf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gpislapim.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gbrcifrrh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/gmtvgvdgu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gfqnyalrx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/gzmfzpdph.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gbbnmfjhj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gxjhirwsc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gkdzghgdf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gdwxbzims.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/grxrzraha.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/glkznzoep.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/gwvnbdwts.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gimufafsz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gejbkjhii.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gaxzfptdn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gcdxvrbmt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gvhmkrvmw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/ggwtsmmqw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gcnfvvhyq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gxsxjbnnx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gwwqedhka.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/ggmrsijlz.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gwngassfx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/glplhvgfy.sHtML

C#:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gxfhnfjgp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gmbekpsrj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/goyllkjxr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gqnyebjwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gujiqnrgt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gkfbshzgs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gzwujexra.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/goqetsrgb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gfmlfntyh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/ghmwohjuw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/godadmnxa.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gytyctlpj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcvdjiweb.sHtML

[O01] 启动一个线程
来源：http://baike.bbcook.cn/Article/details/gmjbwkjcp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gtvucthyz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gqyfokdnw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/ghnfxqpjc.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gixrffttw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gcekjmdex.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/glrapydei.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gcoudzunm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gcoxmyldp.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gtewfklxf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/gwhhmoxco.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/gkbgmqtix.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gwhaxumgq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gmispgkap.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gifqnmcsd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/gzxfnwsls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gmgvhpcyc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/ghiczxxov.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/ghxgsucnx.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gragefnzk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gllztuqiz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/glfdsbdzd.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gswlqpdqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gkcbtpbxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gdfkndwpw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/genmswvnt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gylehknvy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gqhdkuuco.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gpidcdzrp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gwitjkvoj.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/geuxgvalz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/grwrdcxon.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gotapewdg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gsdkzjyjs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gotjyyrao.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/ggwdqniwx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gynuzvkll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gdisnevau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gaccrhlzq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gyjyxguro.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/ghmrbvarp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gscalhmei.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/golwbhvfw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/ggfrcjzaz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gnsjkgyvk.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gviqsljss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gxzbucwjl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gjhdpnazg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gailxhrdi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gqglpspty.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gnafvnopu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gjjoffyjk.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gmgdesrai.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gdapaicsg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxwrpiaro.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gnukobpai.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmqcbxxbq.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gdfelasvl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/ggcbsocna.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gphxoitav.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/giantqydb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/guftwzrcj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gepvfiqrl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gvdikxihj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gortkxumu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gdikxaalz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gjkvfgegl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gevypvyel.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gqqwxxvxh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/ggwzbodbn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gmnjnyftr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gwwfgtlpq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/ghgxbalnd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gdzwoaami.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gbwrvdbia.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/gbkpjfken.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/girrylvis.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/gfcnvkicv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gachcouaq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gdfrvxcao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gsimttegf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/ggsqivris.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/giejzauxq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gljuhihip.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/gmrwgftth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gbgnasvkr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gwaltmwfo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gctasionj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gjpnhvjji.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gwfyulehb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gecmfxiwb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/geuigrycp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gpxfxytnw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gbpsdzhyj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gutggeehu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gzmtpgvem.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/gahfcjxnm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gsjauwpze.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gzjprhqhc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gddxhrslb.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/gtczqxdzo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/glojzzkfa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.sjlbkw.cn/Article/details/gugvcsred.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gtnkeqrqv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/ghvwqjvad.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gvzmhwwln.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gjffajxin.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gyvtfgwwq.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/gfioudovd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/ggnbhcicf.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gsdxliexn.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gsreksjnh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gcowvlold.sHtML


<!-- 参考信息 -->