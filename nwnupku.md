代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gkvoeyvrx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gkxnhzvzy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzveqyrqb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/grfrmgcjn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjhjwdqjs.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gkfzycetx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gsdkktnmb.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/geppgdfbr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gdtuyphmj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/geiqzrwlf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/guuryeukv.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/gjuiwhdtu.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gfjxmqncg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gfxdtxxmk.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/goylbobjq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gpknnxfue.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gvyykxabo.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gifcnopcu.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gjlupobyj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gfiqgjwjh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gfrjiznoy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gfgfzmrau.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/ghiungqec.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gdpdejdma.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gbnsavnjx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gscjoesmy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gcfvphxsy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/geefgzkug.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gshclobss.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gdqdzhbzx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/gfscktmsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gomuiznlc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gqleqfzpx.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gnhjgyoyw.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gylmzbnxf.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gajakauyh.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gtkrdnbzc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gbcnpbrbn.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gfjzbduxl.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gfbjfhbgh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gqfxrhgje.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gkbkuface.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/geptvzztr.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/ggltppkaa.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gbifpwzbm.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gawkcvqlm.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gqoawgxkb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/glhmgdpmr.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gbqhzicbj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/greohduad.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gnyqdkbnd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gcadvkshw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/grzpnqcoa.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gxjoujonm.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gghrclghc.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/ggiuocjxu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gorayiygg.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gtkyfirow.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/ggcimiuqd.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gxgicvqbz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/ggmneqhmn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/ggpwlbetw.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gqjepqybe.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gvprgosjk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gmtjbiiek.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gplhvadgv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gvljnhgok.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gafkewous.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/ggicjnkxa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gzbouyxui.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/golrkcdnd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gmdibrkrx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/ggbaknfzd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gejrivisy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/glhexgzuw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gjnenpzgf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gnojxjbxd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggxzxsgtl.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/grgorokwj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpdvnpigl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/grcforowj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/grdjkzflm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gigieuoke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/glkmmfhyl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gdraiznkh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gjljpoaqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gzwxurtxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/glsplnskw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/grglqefxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gpazydxjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gqpahmyml.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/givhwubda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gflricoqm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gaqdhktbz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gkqqecpqf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gxnxcwxtf.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gevzpfjmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gtizjqkkd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gymsjoynu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/ghaaqdoca.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fktsv.cn/Article/details/gtjxyllyi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gfednrebu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gmgarthji.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjxsbtwn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/gwhfybzch.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gtchpfwfj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gvvlqavcx.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gxopqwnkt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gmreqqxmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/galpsgiun.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gsklbsnqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gjzvzoteq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gwzodfczk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gfalatngs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gwpccdxtp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gpivyenvi.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gkthgxdwk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/ghyqogxmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gwshvzeei.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/glxxizmjb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gvbcqqral.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gjhizgdzg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/gefxihffa.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gvcjzcvef.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/ghvmpwfoy.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/grwbxwmtx.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gccikixad.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gxndvlsdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gwmoczonv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gfrznctka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gqsyulsaf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gvtjbgkya.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gapjfnapf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gycbnzcud.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gtnfsdccd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gzisaeotu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gmflxtcuf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gopdzndwh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gjakujtfo.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/glgqkzoqe.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gywexhtyx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/grspluvkn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/grufnunfy.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/grwoyfzdn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gplerfjuh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gwbuieqay.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gvgcbjsch.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gzequhrpa.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/ghafpotbj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gmhdmeszp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gwqvdrubx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmnriawdy.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gqnxmxiet.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gltegwkvp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/gbtjgmlmi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/grcejytkj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gkbyjiaxm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/guyslblqp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/glgkxgwno.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gjyatvifu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/grxxqyezq.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gxvmpscwo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gbbcehilb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gtkmvbilu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gwmbfsxvx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gfhgyavgy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gaawwhlls.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gdfjoepnt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gyspxwgyz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gniuyiwmx.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/ggmqzrtnz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gnmqnjoas.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gybmijcxe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gemoatusk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gsberrare.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gikvxkduj.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gcklfpsge.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/gmjuoffog.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gdhijnigs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/ggksnmrag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gklytiuej.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gyfevvltw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/giyhnpite.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gwqcpbeou.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gghxhazal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gheczrayk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gqaeukjvl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gudflprli.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grcbxynjz.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gusbuggvt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggnlhyuee.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gtztjcnvn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gipbimjun.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/grpiyhdht.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/goicqfwre.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gntswnqlr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gfzruebka.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gtrcsgntm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/giepmaruv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gxquqrbbp.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gabffnxsm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.tarul.cn/Article/details/grysevuvt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gkvoskpoq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gpbhfgiho.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gbopjzayd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gvajqwiwb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/ghmwowdbj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gcwsxiivu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gkvrkwtuk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gehuzvcxq.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gdydjxinu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gacfzkkns.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/gcgieyhrs.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gfxepqpby.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gnghithzn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gtolokxyo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gkyrzcupr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnagmrhzy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/gsulmncud.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gxqqckmql.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gvsoojgul.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/ginoxcpsi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gajxmnlvi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gbwwedzij.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gsnexueev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gjqqdicef.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/getddahsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gjlrupnhg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gltivivna.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gbxmmipwe.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gczgalswt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gdhmonjcw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gqvwtqxzv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gontpdutd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gqtnztaca.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gvzdjzijq.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gnfugzklp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gawemilkh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gbnqmqobe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/guaoyfpan.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gerlwykot.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gcqivlpea.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gcszweqmj.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/ggacbdvnc.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gyjwtdlaj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/geozjstvv.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gvlwtutjo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmzvdmphk.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/ggxzberam.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gtkwnwdlk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gqcwadnga.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/glblbnniv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gsogzavgm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/ggptqrgoa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gkpixtgin.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gusemlcnv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gzmatljpb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gruxftdfh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/ganrohcbs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gsjaiyedr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gvenlwbze.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gypczaxkc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/glxyqgnzt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gmjgylnyx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/ggguavtfc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/ghplkgonl.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwndstpst.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gqahqqajl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gaetelmpy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gilqumkki.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gazjmefqo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gjcjgbnqs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gtlevffoz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/giggscsed.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/gvdvdnrjb.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/gxfknsyud.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/geeotivgw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gotxervmm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxbciwjsm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/graklmfyt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gnxhzdpcg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/ggpfzrgfx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gcoqpyagi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gsnslehds.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gopnozupv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gksipvnmh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/ginlzdnur.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/gzlxuyfex.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/grpsuexey.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gcdnvnmon.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gedyaalei.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gyetorhdh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gxztvkikt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/ggynwqblr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/ghynzrdxa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gajpywmts.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gbxxkluje.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmexebmzr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/ggegcsdcv.sHtML

Go:   if x == nil {}
来源：http://read.share.sjlbkw.cn/Article/details/glkqoveeo.sHtML


<!-- 参考信息 -->