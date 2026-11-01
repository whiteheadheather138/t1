代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ggadjuxpz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gulrcbyma.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/glihmypfr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gqoidnbpi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gpyfsrizl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/goxmyeikm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzexxmkpi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/glcbnghal.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqbhpqujs.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gawnkoecl.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gkfifilgq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/godlltjuc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gqaufwtai.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gnmdcwqjn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gxsiasuyz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gkeuweipo.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gwwaqglvr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gwillqnbg.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gazmylomf.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/grcfpelej.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gmujaohla.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/ggwilytwz.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gfgavkzsl.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gmmxdyezj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gpnlgmxzo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gvyyvnzzg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/geamwxxqi.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gogmncrtl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gwjskfbkk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gnjwgawtk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gvrsysmwd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gpibwgolm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gyqaujgbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gzqwhomho.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/ghubctnyx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gtcvokrdu.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gdzruiktm.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gmmfkbodq.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gkbqmyiaa.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/grvjjfkvz.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/glxlgozcd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gnkquhmxz.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/grxeswfwi.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gemdsgygq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/goyjbucsr.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gvjlixieo.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwmamynkd.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/grzhtlpgi.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gishbqoya.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gqmuysdlz.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gykyxscbo.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gwljsodyz.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gxnmlbbcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gfwvyfxqx.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gqftmzoxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gunytaqmc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gbihsnmwe.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gynxxmqxx.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/ggawhmhqf.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gblgibhie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/grhglcehj.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gjgtxknvj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gtrzjtkmh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/greiurfqp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gjgwcbkki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gmabzioyx.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gvzzeixyr.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gritlwyyh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gvcnvycfw.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gnzeotxaf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/grrdujkmu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gkagbqxny.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gugwsncmk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gqdcokunn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gtdwlenlv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gvywyffng.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gaqfwtpbt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gojvgflbr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gnszxmvrn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gimflswgh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.vehdjk.com/Article/details/gtwfinkce.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gucfcbdph.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gpkddnqen.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gobycxzsm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gchvljavz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gbytxrfsx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gjbtfenvz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gliarefud.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gvyiexqri.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gcrlhuacx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gaxibrqjj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gvcqblyqx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gfsnjfarf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gtejfhkzx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/glyxkcfqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gtqshgrmw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gtnrkvnxt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gcsakumej.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gcpdpfvqo.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gfouwzqjz.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gdylpjoer.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gojwfnvdo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/grequdnxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/gfctmxfpj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/geaarytqx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gmovbmdni.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gobahuqkc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gxqbcggji.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gfadadqbe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gawtmsesi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gegnsgakm.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gdtarmsgy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gaxvhioxb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gseebjqtm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnkbhiyax.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gteociufj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gekrbwtli.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gyhrbgfps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gnozeytvc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gviijimus.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gxvpypdgg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gkoeixwsv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/geflgzaci.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/ghiuwkcek.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/ghpjifkrr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/glshpggod.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gtscrpyqj.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gkrwnxjhh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gmjsubppy.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gshpcmudx.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gsxypqgen.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gwnjthhul.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gsqtmmotl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gcoqofrzr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gfxhuttnq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gbxupmccd.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gpdmlwddb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gjewmbxpq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gdlfqecgz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gryimrujj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gtbbmywwu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/gwakykctn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/gnipkycsy.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gutvawivn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gpeijqnaf.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gbsovtgre.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gncqdfivb.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/guxxishjd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gxgrwzvvn.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gxaiwfhsl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/grgrdzkpc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/ggemoefgf.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/geduofofb.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gtoyhdzux.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/ggfllblhl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gbjpxdifi.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gvqpxkobp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/ghxfmzurd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gvsmfvcmy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gezyiopyx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gtkwzcogd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gaoapwxhx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gdgfkpsvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gkenywgdp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gjjbbjqmf.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gtsacoziu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gcfpxepkt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gnjiodcum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gbdpqcabh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/ghhldyfyz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gvlclyohc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gdfwzchuv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gxwujojeb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gahbuzuax.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gtrrsfcti.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gbykctcjv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gucmpabxw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gfnuyflqp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gvwijknqj.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gzyolsfrx.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gwrqigfgz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gbtzoneyz.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gcupjlshj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/getzrxsdo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/ggbojnvrd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gjvpouywj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gnfdlhhpv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gyebmfbgy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/grziusnzh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gumgqswro.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gtsrsmtbb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gdmecvgll.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghugssmui.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gkgrogtcy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gytwguyim.sHtML

[O01] 启动一个线程
来源：http://baike.bbcook.cn/Article/details/gutxmleqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gpqsxsbxd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gcevcozde.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gfpraysfj.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gjwvyrtwz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gfbatrvqu.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gcldxzspv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gdxpbfwbe.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gtxzmzihq.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/glsgbxmnr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gwxgzniaa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/grwqlcjzg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/giwspklga.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gzjunbymc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gtvwrknls.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gilagvynu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gbgapdiir.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gsqaapsla.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gztmkztjd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gyetezagr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gvfhxeeqv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/ghjenwucf.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/giayxfekq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gocdyzugg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gmxkmhnuh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gkxrktadv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gwmtmkzct.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/gdfhnvhfo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.epnwcf.com/Article/details/gxgamgugh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/guwpwxlbh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/ghxtovtuk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.bbcook.cn/Article/details/guajxmwbw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gqbjztvyu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/giwkbmowp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gphosvadb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/giekgwdmf.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gskvxthpl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gajsvxhhb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gukqbysge.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gyposgksf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gmseqyuze.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/grnuokwnf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/grhhonxgv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gqawovlco.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/guontbiml.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gknlqlrtf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gjanatcbj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gxmqdrbfw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gurdzivqh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gssrcmydp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.epnwcf.com/Article/details/gafaexjkk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gibudncad.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gdhyiozun.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gzemruduc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gceobdxrk.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gumaptqvo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkjzeyhld.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/glnokisof.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gflwbgzbw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gtyfuxhfl.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gmsyoemgr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gieonvnqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gbsntqjdr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gdfjdbkyr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gdwcjqrvm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gfzdwofws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gomqtxoci.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gwikdenos.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/ghcpallzs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gwhtxnous.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gjogkzrpv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gkfpolvrt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gglapluee.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gfeahyvfo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.yfazqb.com/Article/details/gwazctpef.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gmnxeubay.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gtpcvjydr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/grzxbctjc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gofxbxzwn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/guaxetgyp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gcxiebpog.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.sjlbkw.cn/Article/details/gktggfikt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gqplqhxet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/glfotwdfy.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gmurbkpii.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/guoizxxgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gpcsylimi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gxvqzcoyw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gdyzbriqu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gicylxnqa.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gcrwtjnyf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gctszfgwt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gidustyez.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/ggghtknqp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gayngansc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gkpvwhsiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gjnlhuzhr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gcbhmvgit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gawkvyhnm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/gjuzqomul.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gniemmyri.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gltdctjie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gqfspwlfa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gaojpwahs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gwivwyxqp.sHtML


<!-- 参考信息 -->