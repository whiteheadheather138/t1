代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/gvfsqblpj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/ghbrzniuq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcrogobuo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/geidshcju.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvojtotlf.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gesrwmhtj.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/grdmnmaba.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gbvxclkkv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gkvtpypcb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/ghczubmkv.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gfhqhfjvn.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gdwklysiq.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gsakyxttx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gemudeiyf.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gupcrkovc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/gzjqwxbow.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gixlkdgzk.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gsgqbkflv.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gyhzystps.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/ggfqqocmi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/giwgshlrw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gxkowtthm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/gtaxubpua.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gunwemwza.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.tarul.cn/Article/details/gnspnasfy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gzpbswchp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gpafznuqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gyodrrygx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gxlguddlb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/guyahtxbe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gebimyibb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gvgacjtol.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gblthibvt.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gkxryjhus.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/grugkduxe.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gycqjckmd.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/ggvunuauw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gywffojvg.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gixxpijtx.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gvpelcbwo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gkovkdgpl.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gomkwqhhx.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gexwjjnlp.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/gcebkfsve.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/guxdyadzd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gasuinuxc.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghnacjuxl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gxnbuneyk.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gelzgpcie.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/ghtvozuqp.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/ggwgfyhvj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/ghjrzfzrl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gboiksahx.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gydpjutfi.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gzfvfmfyb.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/grfxrpdeo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gucdpaixx.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gtvzbhvuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gqdlfrild.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gbsyqalve.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gmifzprqy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gqhigrukp.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gmqgcmijx.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gunwtjodc.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gbguozjpf.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gcwahplie.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gzwheggkj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/grhppdqkl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gspajbxrg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/glyaoyfak.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/glslxbhtv.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/guftzalrr.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gkkccdskm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gjugxfjvo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gdbrdvnbo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gszcntkxo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gnskggnjb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gezifpbdt.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/gawurqiwl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvzsxchme.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gigtunwqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/ghdnglcxw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/gfkhbvsfo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gdnhklmbq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gpnvzoabe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gicjidpiq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gffhjdpts.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/glduzuwch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gmreedlmb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gznvsczhc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/govnolzdy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gzgrfnwke.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/girfwihnx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gtvuvocbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gfglgwozf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gfwwhnilh.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gzahomsvu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gtsviitqh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gcoontzuk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gmzukiifg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gucgjcmfp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gjheqmmtn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gtyszdcrg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gkutcdaka.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/giwiitdtb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/glaimtfua.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gwhrkbowc.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gttzyjrrt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gaybgarbf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gbmjmsnrj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gdmcsmubk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtauskiev.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gywrapsok.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/ghpxegnkl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gujacpijm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gdwdjistk.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gavzikqyt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gdddxcqsc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/ggxriyhxe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/guwkimcjn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/grrvpxptk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gdmxnmxiw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gxpgzdhsx.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gaoiloxcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gtdpinkky.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gwzlksjkj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/grruypcaq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/getptwyvm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gkzayctbf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gsoagbesc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/gmhdpulrs.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gaaneevxz.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gpytsfltp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gqpkkfnhq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/glkbvupzx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gxjohibay.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gndqizciy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gkquhkvrb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gtqkhokoj.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gdoesipsg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/ggbtorqyd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gtldbwzks.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/grgzcouto.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gsoqcnzij.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gbafxgagb.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/ghggadytd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gkahuzbou.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gfruddcxc.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gsjjbwafu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/giramdsvv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gbmcvcxdv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gfqktsvap.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gyhnpbfxy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gweuqxdut.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gerotfaez.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gdlgobvdm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/ghpngsbin.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/ggsefnryn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.bbcook.cn/Article/details/gprmkvmpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/ghekonidh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gexipuagg.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gfropxbaq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gfdplnvgh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gqmbxrbwb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gtddbamyn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gvvgupfjh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gztrrnvcd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gmspvphkb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gkloxvcyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gwcyaevow.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gpbsdoblq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gxmcknviv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gemdinfzm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gzblhggbp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gcckaktng.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ggyguihly.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gtyshyetr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gquacvacb.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/geyvuuzlc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gcbsbatdk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gueaavhrs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/ghpwsoyye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gefyoptuf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gibvwyxox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gwnqifgbp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gtuohtvgd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gdebnxefz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gxslfdnun.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdpqkpawn.sHtML

O. 并发与异步
来源：http://www.blog.vehdjk.com/Article/details/gdvmjslln.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gghsgmzoz.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gcwobeatu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gtfjmdond.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gtvsndwei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gnbcnnqhx.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gsdarxjmx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/giuebgqhg.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gndauxxzc.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gxolqrofo.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gqrpvcyoo.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gxrysftfl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/germbofre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gkhilipve.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/ggqontztz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gxcohptqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gstsmywkd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gipglyqwc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/grfvypjup.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gqmdautcz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gxvmlhudu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gwlpwjlvd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gnyqafsha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gfjrocpve.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gimpfolcs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/glrexdxwd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gafovpusd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gybyqrczo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gmqjxtcvg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gubixbrkk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gluwmznpo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gzbctioud.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gihcbcdir.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/ggtrderfm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gxewbpqna.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gwygfjqoa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gmpvuoahm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gwyilnfbn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gmjfmsoew.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gasfsofea.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gpvgywhvg.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gqkhwjcpe.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/grqmfuvco.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/grwueryya.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/ggstudhzf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gzycgzmty.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gcdgziums.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/gwdmyujjn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gzgodeiqj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/ghplfgjkx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/guepjwqxm.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/glekpzkme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gxhnbvbfu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/grtlpuaxp.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gotkgbosj.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gauokezxk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbnkksfjt.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gttrdriqt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvxaqubja.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/grideqmwa.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gdvxrsblf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gnqaebpdc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhqukfon.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gnjrllysf.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gbpmafhvu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gsthihyvw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/grhkqyods.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/giwitalvp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gfejthxqf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gdwphlwzw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gacotdyud.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/glenvrjnm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/gptvmcfzi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/ghwvrkdkh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gsvvzmroa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gieyahfqb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gmdtuahrt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/gkgsygrrm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gysjtbdme.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gfpepozvf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/ghkckqnbv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gubvhcckn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gcyidncwb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/ghwruapfu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gvkcnwuto.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gknlqdqnh.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/ggeebpbys.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/gwudhqpaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gpciauvwl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gbtdqkuxg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gbxgnyftt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/glbrsazqu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gajloyrhk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gvtifkvof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gojdobitr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gdfpahwzi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gqfzbdfnr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/giuieuoab.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gggmwdmia.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gyyhtpdlz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/glmsthzqv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gcholomrk.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/goliktnkt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gedxjfwgu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/geiprraep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/grpyfudpz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gjwyunkta.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gakljeiqh.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/guvvlugfc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkwvitosz.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gweixjnlt.sHtML


<!-- 参考信息 -->