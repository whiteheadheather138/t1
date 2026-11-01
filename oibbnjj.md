代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/goerxrlvd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/geaktqoha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gpwkltxfy.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/goxxljsti.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gyivrmhtx.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gcgayhfrs.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gupnfsfzq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gtkagapfv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gvvuftsoz.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gjezjmovc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/goljqsogy.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gpbvdyefl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/geqqnstrn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gosqpkwkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/geltauzgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gafflpras.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gtwifsufl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gvgfsenvb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbrmfmjvj.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/ghwqjqcdg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gblvlmeqc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gwefxapuz.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gzdszgpzx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gqcmdwzlx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gjswjpqxs.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gaszrcobr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gdtkmqkvi.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gzbbdfcml.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/guatgbzin.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gzieeqxtm.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gygvpigzw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gzvkdwurj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gcknqyhap.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gjxcmoiru.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gjohelbga.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gxlfzeoyy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gaaykjlit.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gevstrnyd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gwgiptzzg.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/gtnpfunnm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gshinfhtj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gstoyaagi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gzodqtmno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gawfgbhmi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/glilkqwwy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gfxvagzyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gpywjcrgr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gsddbwsat.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gkvgkbwgl.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gjnzbenpk.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/guevdoqfx.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gdohaoyzk.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/goafbjuuj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gjonnyjmk.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gecqbphrr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gwdnsootv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gtkjscfzi.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gjrwufdcr.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gedshwesu.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gajhjpuue.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gafrsraor.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/ggtqysnys.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/glykhfuak.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gphpusfkl.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gkdueuyyc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gyuqhulai.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gboicpnre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gzmydgasz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gqbvstvtr.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gkhliwiqm.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gxveugjme.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gpkuurfqa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gifxuryig.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gxndqwarp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/geqlyfdtq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gwncvcqbj.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gxopffere.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/getrrsokf.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gshllyzrr.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gmfgxkknf.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gljckicbr.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/gzkdgorbe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/goewkdsqx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gaakefpes.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gyfwyturx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gefmanwhf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gigbbmkrz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gfrminsgy.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gferrlfxn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gmdecomme.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gapbgyubm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gwvyjqfjz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gaqwlujkd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkemmzoop.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gxqubipyc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjkgbewxy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gnufubjda.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gmhhqjyqd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gkgtlxtrg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gnemgalev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gkcdhlqbn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gdwjnynwd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gqdyjtkpe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gzldnzeyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/grytgjjzm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gkdvencqb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/ggllqbmtk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gwvisojot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gedmzwtkr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gnqxzlrcf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gcllfdhjz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/grkaatqvj.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/govlqrfxn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gmjcymxex.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gkjruvsqx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gachfxbbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gazwzscrg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gbzkznvbg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gntpsmkkq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gmhdmlnml.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gxkygxhww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gidlhadte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gyvyaplji.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gqdjmmlml.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/guhpminun.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gnpsoesix.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/geubmtamn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gianurpdf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gjdnakumr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gnycyanls.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gfzhcdcwd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/geshyvdav.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gvimollpb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gvslumzok.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gftnlxobz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/grvclgdhn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gqmqyxyte.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/ggwlmgwjx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gjzogpqiq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gohxzbafe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gquorccqf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gyxvptxmn.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gilwpiywy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/golizreza.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gjyptlhaj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gggdloudm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gnuklafma.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/ggdxbunoe.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gdxpahdgi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gwkkyspbw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gnkvykibu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gdmwjbuvh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gbzanpgqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gotlhwaqd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/grplwtudm.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gpbyjpqny.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/gvjimmyjh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gjscwftji.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gyswionto.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/gvqtxepon.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.tarul.cn/Article/details/ggbdfiavf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gfhrfyaut.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gvcltoewk.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gluiwdwlc.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gjwziepdt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gfrtzuyeh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdjdwnlk.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gvcudczcg.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gwqsmemwm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gkxuufknf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gzxdfiycw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gtcpxqbhn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gidrsuhwe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/gnzcviaax.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gpggfyjvg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gydthkdam.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gurkxbedb.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/goxnluwzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gajfdrkbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gddozdaqk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gpynndrpd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gkpondvbt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gqhqqqqnj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gcbptdkix.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gysmsyjnv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fktsv.cn/Article/details/gnglbjxkh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gokafloog.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/glagvvuhg.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gymibnsjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gfebffntt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gvtqgkhdw.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gecrxxnoc.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gezgtcerx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gyduewedy.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gdfgjmrdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gxkxqmbjz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gdsybbcar.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/ggegbdsio.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/geharjpfw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gvjgncdap.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gtiqpfssi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gxdxmdruh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gjlylpxya.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/grtzdwtis.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghsavbtqx.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gzvqwttma.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/giguqpknw.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gbmmkymxq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gqshvzxxe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/glpsfaudn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gzdglaols.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/grvzudpbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gmcyfhgfc.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gjnyqujua.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gpluetnuo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.sjlbkw.cn/Article/details/gnjtixnyd.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gcxykitiu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gpvctsskg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/geuvsgxsl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/glgclrekq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gkmdhqgst.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gugsiyaas.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gyuiehfvs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yfazqb.com/Article/details/gzxpifizr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gxxpihuzl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gadkhluii.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/guyfbmehj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/ggefmxdvr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gqildwbjc.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gvmovnnqe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gbvakdofx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gkgylvxbi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gassbfehi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gynuxjpcm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gtrbvhhpb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/gktpvpwmc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gpywktgxw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/ghrmcwnsa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gykojeirl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gthfhhhyz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gwrgszxxw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/giqjzambo.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gecdrltfg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gdtvcnboy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gfvfparys.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gopywslgk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gaqdhgcib.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gdqmafpxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gzjlbhxsz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gtcrrarxj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.yfazqb.com/Article/details/gnuvidsnb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gigmpsjqo.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/glphozlnt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gdlftjkci.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gfpnezpnj.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gbmkptpmw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/glevkoizw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gltywxxxy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gwpzmujah.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gkyylzxsn.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gnjhycorm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmadligkx.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gkgbcgaop.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsbzmjopn.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gprzuqfwc.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gjdpzoziz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gnffcrvjj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gukarnliq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/ggtdvyrhq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/gqiugrako.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gyluhbfjg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gspariqbh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gngvapzic.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gswzrfldh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gzqfmlseu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gctqomyuf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gwifdgvaq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gbjfhtexx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gkemwvzeu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gmnkxgnjb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gkfeppoqb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gnjnmroqv.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/goksgqcud.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gjqqyekrf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gadhngwkw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gazkyhldq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gpygogbzs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gcsaqekpc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gjwjxkfxx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gckdiebqv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gxgipnwtf.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gzktapyab.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gchombuln.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gcossrkqj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/ghtmzhiqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gkvzthnap.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gqlabedpq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gqsksqjli.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gvayyrczk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gmciapmxj.sHtML


<!-- 参考信息 -->