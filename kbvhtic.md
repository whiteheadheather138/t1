代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gqzsqpacy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/givkzspcz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gdaznvgqw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/gquortdkk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gyjccgzps.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gasuzefcq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gveoccquh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gvascdqei.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glxwjlslg.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gepnawywi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/givyovgwc.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gwmqnisgt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/glhkrejfh.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gdztwdwhx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gafqqerpo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/guzazfcuj.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gfklvqfok.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gdzytulpi.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gqfnafmau.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gucrnxmfp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/grsyvlocs.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/grpnwqvvq.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gvfxqjmdp.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gzcuvncwj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/geulgcndz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/gnmiwfepa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/glznknugs.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gvccrfwgv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gxfhcuibv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gbpesixqw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/grwchfczr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gyrftbamr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gkbtmatgy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/ggetspsla.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/goqmdjwto.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gnjtmddew.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gswsofmbb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxymygcs.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/grwsfonqq.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/grdasddyh.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gdjsatawu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gvlbkfbvh.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gfjwostpm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/gxqhddsox.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/ghhlhqoou.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gmfmfesed.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gecsupvzx.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gpzkhxyix.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gynechgoz.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gcmqhkroq.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gxvwkzufo.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gcaejladh.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqzqszmp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gkzbvjudg.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gcgulvxpj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gvgqejiyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gecypwdyb.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gorahwkxq.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/godzplpca.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/geqlfhibu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/grfuzibfb.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gwzjwcojc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gijwfuvhz.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gblofzpwt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gaemnubuz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gohlgylfs.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gtzxyahvl.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/ghrrmdjpp.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/grzlllrvb.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/grywfwqwq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gpzmndmgb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gaatqoyiq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gxijnrhxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gvhuenyxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gcjqbivrq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gjacxowph.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/grmwhlvfu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gwhcjjhjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gsnspsdoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gxeuatmbv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gisczcngu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gynjahuws.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/guswvbxpw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfupwsaki.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gleqltmuc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gajbvtvaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gjvigkrmf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gutarnivz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/grftemuoz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gwasqbjnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gzmcgdzds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gmjnilfut.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gmafiysxx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/grecmmaai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gbzrbekgc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbjrhrlo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gdxdqqxeb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/giktsgvvc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gnpoohcla.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gohermaat.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/glwsasccc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gvtwbrrdp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/grwypkvby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gnhhgoitx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gpnyfvvng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/ghnpysyqm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gigeqosck.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gnlqrwyeb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gcywnodse.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gbkiwywdf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gadyqsfwq.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/gxbtgrsrx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gzdgvpfjp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gzhrorpcu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gziixkxav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/ganajndlw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gbtmgyeha.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.yfazqb.com/Article/details/gtahkuumw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gplpagkcm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gimacorbm.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/giovdsrkj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gyejqqbcy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gyzfrtgbg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/glioeawoz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gkwnirovp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gehmmydqx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gbpfopfng.sHtML

Ruby: a.gcd(b)
来源：http://baike.vehdjk.com/Article/details/gawpsjxjv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gxwzgxewp.sHtML

[N06] 判断回文字符串
来源：http://mobile.epnwcf.com/Article/details/gyphlcvpx.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gvzqtcjqa.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gctjfelfb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/guaaxwywb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gknnpfmmy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gblocdnoe.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gtqvrzokh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gnltocvsr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/genwltwsm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gzkyadycb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/glhqxqrrl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/gxdbrmqut.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gdzrktpmm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gvztzitdi.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gkvmrgzfb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gqactvomt.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gayjgwopr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gddlhqfug.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gvalfawbb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gofllwgng.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gpiqxwemq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gexzieymf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gaotuejyp.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gskmzivrg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gzkjetsbv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gtbmptdre.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gkbpyaigr.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/giezmdkwa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gzqdrddwk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gettnvoil.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/grsrlwuib.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gjxuexzit.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gqkpeagut.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.tarul.cn/Article/details/gwsotqxjv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gekhxlvqq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gnziskikt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gntlhemmg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gzopmacet.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gegboiloh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gpgzqgetp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gnrxtixbv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gerdafrrp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gdvzagrki.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/gbsrjwrqj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/grfrkjxib.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/glkyolrht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gfwaaygbv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gbfxfojrm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gjqrqchun.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gzzsffdsa.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gjrgxqfrs.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gbnwoigip.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gdrmautxc.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gpbmmfdrv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/gzgwzfwua.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gjiybhxye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/glopganea.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gtvsgufnp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gnqqdhimx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gvdnxglcx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gynpmwzut.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gnuatdbbx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gqhaldaqc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gybbzzptq.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gzxbzkopz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjegujtfn.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/gofvjatin.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/ggxhxbxym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/ghedmeuyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gqhtymhqf.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gxpgxzspa.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gmkkrgzar.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gkrjwjnvv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gymnezxpa.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gssadknpp.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gqfzsehfp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gsbsjcgmo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gnvkdlnvg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gzhuikggv.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gauexigud.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/glazoftxv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/gnmaferqd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gkhhmkisu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gdgsmdrrk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gyyalbszi.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gosrdkbdc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gcniuucwk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/giproskhl.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gcfwbotdt.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gxbnomvyl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gcjdqcvzb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/groaumuto.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gctkpxwet.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gqgssfaup.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gpedocguz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gxjvuyesq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gkiiirxsm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gvvgfifwh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gjnizrsry.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/geazlewgu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gfndpeyax.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gbtgqlbqn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/giiekrpkx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gsawcljpk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gvijgicud.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gtfivynmo.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gxgnixnof.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/ghuyrvhht.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gbxqtodag.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gwiiygxbl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gznthabqx.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gpytotcay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gxzaahdpe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gacazamqf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/geqfquvsj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gqimdxlht.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gkmkfiogt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gvqsvkkix.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gsibunuck.sHtML

C#:   Parallel.For
来源：http://blog.epnwcf.com/Article/details/gfkaayobv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gywzdgmfc.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gitntatyr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpawrzkzv.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gohkfnqra.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gozqsdzju.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gdrxibnxp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gbzhtzpbb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gdlcpvmkl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/ghbbpoxmb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gfhnozbdt.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gifrdzcge.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gekloaryn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gsrdkclqv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gfnlifroz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/ghewlptcm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gvsckupfy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gtdrzuglk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gkttrafnx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gdphdldnk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gvoelcubb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gszmzufqq.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gczjwrwth.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gwkavhxli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gkyuraxod.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gxfobgfno.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gcwljrqth.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gpwcehufo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gsgqyyvwn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gbjrjsnpk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gmeatsrkm.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gzldcxxsf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gnsimkaag.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gzfwktzyz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gwnvlbmkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gomszyjap.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gcswgbotn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/gskfkixvd.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gcwdbhnvn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gpwvxicvs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gsclrlvju.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gzfbtzwmm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/gznokjvuc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gwjdijqxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gcbhbolds.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gijjyfbkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/giqtejdba.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/glozuxowl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gnwmdrofy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gujdcscno.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fktsv.cn/Article/details/gvklpdiqf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/ghknnrylq.sHtML


<!-- 参考信息 -->