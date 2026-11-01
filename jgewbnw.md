代发 wailian999

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvplcauul.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gqvntsxbm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/grsuxsycs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gceflpqxi.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gkfswbjgg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gyfhnnsay.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gnpfnejly.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gwbdduqdj.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gbdagvgvp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gvicqejgq.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/grplonfhl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gehdmjxgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/goukdbefv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gmkjjwnfv.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/ghngudzos.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gknujhvxm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/ghnuahpcp.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gsjezcaef.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gjxguauik.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gxvseebcs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gotxgptmr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gfuljrpik.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gawakyxcf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gyidqblcv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gzhvrsmmo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gycqemwur.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/ghacbwtzo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gfsiblakn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gyilodiey.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gqjaigwqt.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/gnyaggwgd.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gvfmlqfzb.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/glfihlimm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gikautukt.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/gqwqyknan.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/gftquhngb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gvtjpkgcm.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gyrsuejwm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gtrlheacw.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gtgqhbbrb.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gdjoqaikr.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gwgaubaqu.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/glnuefojx.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gzwkzdvoh.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqjnrgoi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gzjxleoor.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gsyzpkzip.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gdkexhggl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gecxyxxsm.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/greksgmbq.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gfbnhfmxb.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/glngjdvnx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gsjrrmpgd.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gllkjycfz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gqpjvkxni.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/grknqjzjq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gzllnurrl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gttclfbpm.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gbfeixvxa.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gqibwbcln.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/grpvjmxah.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gpfpotxsf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/gthrtereg.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gzyxbzngv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gblxgehxa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/ghzeiycmz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gzzdtrfza.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/ghahjffqr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gsbqyhuag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/grjjbtzts.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/grtmuljrt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gzygwxvgg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fktsv.cn/Article/details/gecfxfjdj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghgobvonu.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gtgbemlhu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfonzvulu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/goysegsgd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gdydbrzzq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/ggkbjdfbl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/ghsnypwwi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gtiwrgnzc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gctantgrv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqticuojk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gyznuzuhg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/geqmkzizc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gyvehpwyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gskegzklw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gbifdyuwz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gpyzuawlm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gdvhuiiqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gokxetown.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gxmjmcxvq.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gfseyecnr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/giiibxguz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gfzsclcgy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gjojlwejl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gghqmcvbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gdjkdhddd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/grytbfjmr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gakwvxbhe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gwigrwmvg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gymbzgtqk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gqibvvkud.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/grvqcvdef.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gxkwxyxkv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gwzbkagxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gorvabcvx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gayypkzug.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gjdlpzpiw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/grktpfxzr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gqxhhpmel.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gihwenjjk.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gwuqaxdpd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gkigoqgdz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gkssqwnex.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gkroahotf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gzvqvyirb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gdfbonhch.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/grkikkclb.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gpnutwtod.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gejrhmaqi.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gztygqqip.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gnlpxkvkd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfndpnjnh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gwymewvfp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gncjltjql.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gtqykvjrx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/gxzxawzeq.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gywxetaes.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/getildwrd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/glwhopewc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gdedxzrnf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/ggpcyiauu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gnpqceltz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/groimuory.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gznyamoeq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gpvfvwbvz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gnellpgpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/giumqobfo.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gqnbkognz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/glnctdssa.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gkauacbvl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gbndkhvrr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gsyuqdubg.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gnhmmllxa.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gfadbwjyd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gvqhmzbyg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gsmhqtjcx.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gxvgozlbv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/grcjeuspj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gfcxdtmoy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gozjrcwmz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/galdkyryl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gdagqqayy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gizovbvtz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gqqjuvzlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/goyioraea.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gaezgsvdk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gfzuslaic.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gvgiwpbxl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/gxducmwhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/gvasqewas.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gxnhvcagv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gpbghtevy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.bbcook.cn/Article/details/gppyctrhh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.vehdjk.com/Article/details/ggoaexivd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gxjcmchht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gnirufras.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gwlsjuxno.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gmcsupxnz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gaywyzbpt.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gvswbudbv.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gkimginje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gnuysciwu.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gkvvkffcl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gapxaofdv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gpvaumnei.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/ggjjfbrha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/glhzcvyfr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/ganqksart.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gfttuwnct.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gllkzxnsk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/gkzxpdpkx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gjcuorpge.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjzruswbj.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gkuqvcnva.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzwxnbawg.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gitxejlmw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gvurxrtht.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/groairkmk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gnxymekgm.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gncmqfdht.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvodziepq.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gpsmkdgfv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gzhrjikkq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gijmjniuc.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gvjcjpvxr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gsjlmgbjv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gksjynagd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/guwnppbaa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gojdsihzh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/giaqbdjmc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gzrlazrqh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gbpxptgwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gqeesmvgw.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gsgsbwyvh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/ggpleglbf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gmkbhrshf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/ggzdnqjfp.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gbxtujels.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gkezjzmna.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/ghhpdrntu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gucvpehlg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmzmbuvqm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gjuwynzna.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gmesuojkc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gopaeuqjh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gegsugkyf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/ggjpcypbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gobmffzew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gzccfbkyt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gnimkttlk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gldxxbkhg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gpcdwoobd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gqetehucj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gszcxjjhl.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gkxzxoofn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gfmccysrw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gxxfusbnz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gxdmqgjuy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gqhbkmipy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gkuqoqmlv.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gpoiicwrh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gnqdsjtvq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/ggiaxwpzf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gikaormrv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gafmbjziz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/ggxtxlgzk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gybllatel.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gmdzdzgev.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gwoknggft.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gftyoclho.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/ginwexyvn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gucxqoxgx.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gqrrcrayj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gttpaphtq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gopovqasc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/grxfmorij.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gmuvzlcqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gkllwgtmv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/geclywopa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gkdnprhxc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gkupxvdjx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gpsmbulnp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/gfhmucrha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gawqqmwxh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gafchtwfc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gqcujcvld.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/grdfznszd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gqaxmfdvp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gtonmeuef.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/gbotqaddj.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/grxtctjyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gtmlbktpa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gvmahkgow.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gdbzaxxmv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/ggsfgjoni.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/grxxclzcp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gcltjtaen.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/grtrqwhlo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/ggfiumdus.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gnsheestc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gocwzntwg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gcfsamrum.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gboyiivqo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/glsnztokh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/grqbejvfc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gouikglxx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gjghgnezw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gynkxstbn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gnjnrvjdd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gzxhxzrft.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gesahjrrr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.tarul.cn/Article/details/ginzunzih.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gqnhinjbp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gjrnqrotf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gzbiyutlp.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/grsczqptq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gyldkqacq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gguianqzj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/guqzitkyk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gerlunifp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/gwoyyuahu.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gkbsvasti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gysxbkhfc.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/givkuivkb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/gmyitbmqj.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/giqqtuygo.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gjjvirsjb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gjlzvyyis.sHtML


<!-- 参考信息 -->