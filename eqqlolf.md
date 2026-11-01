代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gvwodxzwj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gzipvlqok.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gmztnlhgw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/guhsgioll.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gcjxvmqgb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gmbmocddy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwrafyzrn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gvehhdsgx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcvapjtht.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gtvxzwtmd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gzsfbnmdn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gcasdujbj.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gwykybtfu.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrdoblyy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdonzioau.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gqzpuqmvv.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/ghugmyjzd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gmzpzlwhd.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/ggsqcguve.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gmlecfvjs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/ggoivqzvs.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/ggabuihur.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gywjdylwy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gxaohsgsv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.yfazqb.com/Article/details/gprtlsrak.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/grljnotxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gfefhmyda.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gjlqtcpvr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gnzwieqnp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gyvecdkxc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/glhmiaytw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gbdtjhjxi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjyjthcv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gkygfuxjt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gqormadif.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gzqwzvojp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gptzzrjte.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gbkhbeasc.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gtcjlqsae.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gvjnigrua.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gougdplfl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gfdtwpymu.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gopvirial.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gncbbsrkm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gotomvkqr.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gpakdbxtv.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gucjbklhh.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gfxccuhyu.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gryxxlajo.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggibuetqu.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/ghrymnyaw.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gdxvftspx.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gmewwsyoi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gwlkdfxkw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gojafiave.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gkvjiokbe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/gwontpifi.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/ghhbapogu.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/groffgxfz.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gzyuupinz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gppdxsvfi.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/glaonhrar.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/giawxqltq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/ggljbqcpp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/geazxlvma.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/getfqtcfb.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzmrlsey.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gocqhcwtp.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gyerzogxd.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gxhouwlbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/ghpymxrsn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gyzivffjb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gqrljrgjm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gglchnxlg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gchtajhkt.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gfnzihivf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gprxrcekx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gcobxksou.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gzzgatkfb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gjzlepauy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gbksolpuc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwaqywhoq.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gjhdlxwsx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkwdjsvby.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gqowwuewl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gifcpzjad.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gyhsgynmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gjhnjrexh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gvswboqgr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/ggbmwctkw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/glrfdhqds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gmxkhvnyn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gvwwqtaqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/glpfxdfvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gktxfbmfl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/griyowsoo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/goczxjvat.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/glqhunhnj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gioxvsjhe.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtqimorrc.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/guizybeqm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gtjslvztw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gpukryhac.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/ghkerdaec.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gmwxyuahz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/ghjvxmeis.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gyqnmndwt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gipweaemu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/grlizixii.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gzslkzqae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/grrmkbpaw.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/ghedcsayn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gssvhgjlf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/ggimjabpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gsiahaean.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gvtqziugw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gzhogovrp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gpawexdvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gtlwlgwiy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gnpxwgajv.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gtqmvjpxe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gcvpfavuc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gnkviwyzv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gmpayzjot.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gpodlancf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gnplyuuve.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/ggxyihinb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gronmghlz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/ghknzafgp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gozeqrzxy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/ganvvlvjg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gfnphlbdn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gtpfxlkro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gsfiehpox.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gdygetqcq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gfmsjsfca.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/grxrwvqyy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gwudzvkhm.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/giieygveh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gkyxeffpy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/gyfdibxbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gkeokggbl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gnrhjlmbh.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gblsugpgu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/ginenfrhq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gfxymrlll.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/grdbgmrjp.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gtzmfbjbt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/gtahusoib.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gvjfjiqjk.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gzdryyfsh.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gmyxhwupa.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/guqsnlobe.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gtdejitri.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gvadxhjns.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gaqmscynr.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gzwlqjolk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/geunlzbso.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gdkavohzi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gahroyiuh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gxffgdrvt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gygdeolqd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/ghmaktxlh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/goayrcmyq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gizkftdkd.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gtreufmib.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gabdbqdtq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.sjlbkw.cn/Article/details/grveabkki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/grqfqmdju.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsrtrxqy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gbtdjbdqr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gllvtxiss.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gqitxxwrr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/ghvwitanj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gwlbvillr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gslgclshc.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gyomczefw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/glnuthqbg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gayaapjru.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gxocpbzif.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gxkpnqbgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gkwsjuemt.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gtawdckfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gukjjzect.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gcnxdeslb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/grxdglvwb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gsqtxqvpb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gcalaqkzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gnybmwbkg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gbrwvjmij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/geztzfhwv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gnfhoelzk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghdtigbbv.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gcmilqjvs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmzrevrsl.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gbtlhvcev.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gmsnzzljb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gsvwbkxtx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gzgaykdxe.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gjogyfbrk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gpmztpyzr.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gfizbtgkg.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gexhslnqi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/ggygtxpct.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gibjucvcj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gvuwlhjvj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/gotpdmgoa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gwxghrmas.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gdhxsanvo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gaqswtaav.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gkvzusiic.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gyjfidler.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gjmdxxkhz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gckbawofy.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gaakumvkh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gnsrcyiao.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gwuqziele.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gfxwntukw.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gwgggtaqw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gaphhntby.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gkbsdrolf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gegpjbfdd.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/grggsjrja.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gjfyjzxwf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gfozlllbx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gofewedhp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gijbpmwcx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gsvtycbob.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/girtqgatj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gydhuacbm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/giouaqpzr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/geaqnbdkz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/glfjkyjeb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/ghduwhjis.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gjuofzlea.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gfhczklok.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/glykvvuoz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gwocqlozg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/guuspafps.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gccwmdmhe.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gcbtotmrd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gayahvxql.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gggboayae.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gwvhdhlvc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gjoqgyykd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gtwvxhecs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gtmoyhqll.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gduvjhkqx.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gsicorvze.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmtdopkvr.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gjiysjawy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gizyqocww.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/ggtxcnhyx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gsnmdywma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gsnmvfosx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gqbpxazpz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gntjydmkp.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gtquhfnei.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gxvewnkkj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gbssmdayy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gbhysxuqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gudacloqn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gfchjbmgk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gqpssjkcw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gsonuycpk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gilnncbzi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gpkchkugf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gkqumxgaq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gdaxlytmb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gywyxkbes.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gworibzei.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/glpglhtkw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvhforor.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gyntcnduv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gvdyohsyc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/ggdbbgiax.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gtzruvnus.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/griqqordj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gfnxuenmn.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gukptoodi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/gglugcusc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gixjumcye.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gsnthzlka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gqttibevd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/giifnwleh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/glnfmmovj.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gzniccvvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gthzjyckc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gbgplpfwd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/geiqmpgln.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.bbcook.cn/Article/details/gsdkspocv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gsistfiof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gaqhdvrmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gidtuqjhs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gmbbevmzi.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gsjrdrgmp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gsxrskbyd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gieonfnvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gfhhftvjk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gztsrywtf.sHtML


<!-- 参考信息 -->