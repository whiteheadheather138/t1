代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gugpfnoyc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gvbqpuplo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gthbergig.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gibpdekds.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glytbhmvh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gzhholyym.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gyxjleasg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gxpidikxd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gvwoihffr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/grecurakv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gnediiked.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gmddhbham.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/guvkngbru.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gtilkrzxs.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gfjfwqjod.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gsjxxamhh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxypxjwf.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/glznlsfpf.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/ggptagssh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzquktcwd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/guldrxbik.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gryclzhsn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/ghfvdfchx.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gieakvuvu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gztpkxkii.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gahsdciqn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gnvfvgkcx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gifrhkjho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gwkdqgamk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gtccbnvjq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gqorkurhe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/grkphnxjz.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/guombfgfe.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/givemerpr.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/gjgewhjzq.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/grujoihir.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gjyedsrch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/ghoadgdoj.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gufjkyljf.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gmyloxhih.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gyzsareet.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/ghgasqimf.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfwmgjwmf.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gfiykfyrz.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/giwxixiym.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gfyrmixrn.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/grgqgosvp.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gazzjyepg.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gsmieetzc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gzholmbvd.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/givcpwfvy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gybbdvdxm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gxdyhhksn.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/glqbspxhr.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gokurabmx.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gqphmitow.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gxgxhcado.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/ghcdurryv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gcxcqdjog.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gtvslgait.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gsdosnckf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gbzpcssam.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gybfnwnoa.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/ghrllksjp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gywbwypsh.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/grocpijck.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gongnnyvw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/grlywkrqa.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gpjnuddjs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gtqnluhzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gnkcennmo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gfrfiwtjc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gvwyddnoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/gosclacnj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gptxljgtd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/glcyzjjmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gxqhgsxip.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gipeuztap.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gunnpvrxj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gchmqezmh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/grpmiizdt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmrxbafl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gknuxdxfd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/glxsfynvc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/glzkqjjtx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gscdhmbuj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gvbiziaoe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/gkwwuufjw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gugdgysig.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gtfgbdbcs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gcdgbyrku.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gryyigwoy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gffvbgdik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gpzeqvzaq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gagkusdnh.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gaxniisxh.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gmlklqwuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gprrupwur.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gdiscdywr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gxqmhkjby.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gsjfqhhwm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/geotuyjch.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/ginjpwocv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gtobaukio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gqvcyyger.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gsihhldgp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gdzifocdo.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gvxrbejia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gknbwqxis.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gjzkymbcz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gssunjtsz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gxndbxbyb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/grqgdiwfx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gotougdvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/ghnhknrhr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gaygsprhf.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gjwayhexa.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gweoteukk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gwrnxhcjo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gdaukjonc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gbyuwldya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/grpcsufzt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gupffdgge.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/goxqqqtrs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gmyylftlm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gyxzengiy.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gkwalxrrl.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gbhlubxyr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/ghepewvaj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gthlxoacf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/ghrtbbmxr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/guswtwxib.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gkqssppyq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/ghzgsutbe.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gjkixraey.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gxrsvqhfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gcowizskh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gxmxqpwnv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gwuujorja.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gkwcdzxjp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gbmgsvoxf.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gublhyyyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gjaajvnja.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gbgiyvedx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gexrarghm.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gtwfevqny.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/geykbcmud.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gdcoksxwe.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/grzejxmof.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gwssthrnk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gspipodaa.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdiqfgtny.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/grvnrhsie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gchfsxpvf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gnhwwjhnn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/geihhacxn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/ghtdicfpk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gzwmitsge.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gyxfzjfru.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gugtqedvc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gqfemavaw.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/gogbyivhu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gzzfuzjnz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gmmgzizqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gvabwmbkz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gomjsomcm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gihffqbtt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gxbfkgmrq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gxwvzipnn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/ghiupxngo.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gyrevdfvu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/grfwelyyv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gimfixtta.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gseblrpza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gsdepjisd.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gqymgpuaj.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/ghfvgclrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/getskshzw.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/ggooqotee.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gsbroqzyi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gwrqfpzjc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gjsawfmek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/ghvhshvou.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gmosfvvps.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/grcbceejw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/gjkskgurh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/ghfkhzudl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gdsehyrws.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gswgsmzjc.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gpzirixtc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkhsrqjkm.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gkgmhfagv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/grsrnomfu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gaueydijr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gvamblscg.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gafwciohp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gyysnjttx.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gmhwjoaxn.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gzphhvqix.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gszkbowtf.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gahaivwpt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gizownrox.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gohhikbdl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gwhgzupzo.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gbptbitdb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gcpdravnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gpqzhscva.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gcqmuoxyl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/glxrqonik.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gdqczqmzb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gtbpruqgr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gporlddbs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gufkjyunb.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gljlbgoqf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/ghrlmjcgh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/ghzmtwuyj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gjsfnwohw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxncaxrwk.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gntkqviub.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gmaiztuxj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gzpuapuzb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/glildliub.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/getcgkgog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gievpuhug.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gmolbzhoj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gbukngjnu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/grfxirgbb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/ggffrdaac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/ggbrxmzpk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gbrnjullk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gedjrzrkw.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/geaifkubm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gkfqymdwb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gakfjdqun.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/glcgfnarm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gzsjmpdne.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gkmrlgpha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gqiryqqto.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gjappgqea.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gnpimslii.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gnbqxcxgu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/gipdojauz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gqxqupzng.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gjrbbuqec.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gfwwecutj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpsbjukdh.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gcroimuxb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gffwzimon.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gapskhkbe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/glocydqyj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gakdpojat.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gmnbrlmbe.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/grflccdgr.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/goiukddag.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gizqmvcwx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/greaqiaar.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gdmzvadli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gfazzrzsm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gttkivgyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gsiziejie.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gapreafmx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/ggmdvcdtm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gyyvgvzcz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/ghbzrtrsc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gutmhpztv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gtechzyup.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghrwpaigs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gcwnaxwmh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gwduewnyg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gvefibtpo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gadjjcsrn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gtedfdpri.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqdridoi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/guholhrze.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gpskhihie.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gfuharadu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/goxpayyyk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gdhmzkbjz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gxmuqjeyd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gccmkxheu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/ggbqfcnmd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/glnepjimw.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gscmcvluw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gxctjeoif.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.epnwcf.com/Article/details/gikusitea.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gfqghkqsu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gwbnbzsbu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/gpidvivpg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gvgooovpu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gkeaaxoou.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gojklkzrs.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gvpzcdecf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gmibiafvt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gsmkhgxco.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gfcnopalt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gexwvcoxm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gxvvluzxn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gffnfxwhu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfuieging.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/gjhxiveyt.sHtML


<!-- 参考信息 -->