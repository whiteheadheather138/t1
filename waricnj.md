代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gffixypvr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gcshzgelj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gyksmeenz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gcqbmseql.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gxnunvuri.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gnjwmjdvu.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gzsczzwas.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/gjqtdsixy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gqovnjgxc.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gqfwcwfkt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gnnmwdlkn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/grggaqcdv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gmslfdhyp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/ggbzhslxm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/geflilufu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/giausfjuy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/giosvchdh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/gccegddmj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjpvitdfl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gprrbolhi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqaiczlup.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gdioximmm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gzthqtbsp.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gsxoapyki.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gevsoiovs.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gjfstbkgn.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gthixxbkb.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gunulvghf.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gtjruwszz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gicxdozhl.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gizouisgj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gkgekepba.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gjpupavwt.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gemuftsqi.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/grvlifwmz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzbxzvisb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gdpebbwot.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gtxxcdxtg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/guwuhqvzg.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gmfbsbwbf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gphaozlrs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gsseervbr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gutduvjft.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/glnosheva.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/gxljyclmx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gxznlbbde.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gqowcmvjw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gwmmnsewp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gjvynvhrt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gqtynimqz.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gbzrdgfpy.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/glzircnko.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gtjmyntjk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/ggremyebx.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gddljtsnq.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gruuprrcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gfaxeshnj.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gzzbnwflk.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gtfohqwop.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gszllawtw.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gvihawhpc.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gzjjolzwe.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gsfebfpau.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gzsfohgac.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gwheyzuba.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gwkpkgbsn.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gjpqyljbd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/grevnoyww.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gztcmzpjg.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gfdvvceuq.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gjymyfual.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/ggwzawzbt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gepmmgetf.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gurofnwta.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/ghbrjbcmq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gamjtduxb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/guupmklhj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gvfdjpybu.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gktvyqoss.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gvcasreol.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gvxosaxug.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gqahnzxax.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gwgptvlqm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gixtwgbjg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gtshvwdhm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/gfhqzofaa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/grtwmvvcr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gdjrofwmd.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/ggjjuzlos.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/ghtgbjcmh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gezrbrgra.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gpzzylyow.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gwpqttpha.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goxltedgy.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gsbjqnyha.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyrmxdhbu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gwoldsysl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwgsqpmyg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/gzwxwpdmz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gmzaltabs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gazvjqhgy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gokgxdyui.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gtiinxkpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gpbbfetpf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/goewtjihw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gopzfzhls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gzjxgfrrb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaflydpmx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gifywswbd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gmznbffom.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gfspqldll.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmimnopcc.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gvqkppaea.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/ghazgjrce.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gypogsohr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gxnapoart.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gpzvkifxs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gtthkigtb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gukwarvgf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/grleijtlf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/gkuqkglhp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gtzjcuhuq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gstzbuppx.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gqtmmqfcw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gkjtnxoqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gyoznlfoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/grvtsfekt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gyfxzaisw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gxwyhdrqi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gjxknfyad.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gqpujnakt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gtjakpsuh.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/grjqwltnw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/gdoqqovne.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gxdcufday.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gomjninsh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/grfpfrlnx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gsgvmsojg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gbrzyureg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gtxqgviiy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gfymcwlix.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gednldend.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gsxtlspkp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/goyeqwmbr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gupalgwsf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gbolykthq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/ghpyrspqv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gqkllmhlk.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gmssqvyte.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gmuqowhql.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gvbdukwnf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/ggcdprqqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gmcsgqguc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gyavhavzz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gfizjrbpk.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gbkjkagzf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gsypttsnl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/geztukzok.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gslkqolcs.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gulwvrwum.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ghteqbsjt.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/goiolkbsr.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gmbaekcpe.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjmzsdxpg.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/grmnjsais.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/giwwbsclh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gvymdpzao.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/geghosbkx.sHtML

[N09] 栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gzoxmzoiv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/grrrphmmc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gkeqekadl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gcsjmcxdz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/ghrrdrpjg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gzenlfsir.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gpzycajju.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gjsrkqglv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.yfazqb.com/Article/details/gighkvbkz.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gitbfvonq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gwouhugwb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gzrxhmqss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gogencerl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gzjkotjle.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gzqcrzkzr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/grzfysvtu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gjygtjawq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gygguhsca.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gccjfegpy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gxostsvsd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gzuwkrtne.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gaqxvcsbh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gkebamtha.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gvkmsldfd.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gexivvdjl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.yfazqb.com/Article/details/glalzgthv.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gagztyfbr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gtmrwhlwm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gcbbieqzv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/ggdiufozi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/ggzyxagch.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gaqchrhol.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gqrcvsyik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/grofzangt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gcmmveids.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/ggwjrrtqf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gazcgckgq.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gtkhjmnce.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkaxekpw.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/golddlbry.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gxbfytqyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gibdjeamk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gwvkusceu.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gszdgheko.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gevjraukz.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gbptlkjwh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gzzpthftf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/ghuyoilki.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gimhwtqsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/govcucqio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/ggbixprka.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/ggvfdzbfz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gouuseyfo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/ggmwqmjjo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/gjlbokymz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gurrwshld.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.bbcook.cn/Article/details/gvkiqvahq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gymvcdoyj.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gezspzcoo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gedtfklme.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/ghqiucjpx.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gdefogaia.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gpesjcdml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gyyiyyqan.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/glpcmgiil.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gcprqtrka.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gzxbnjyic.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gfxcdilzs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gugpneoml.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gnsyrkwno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/ghqyedaln.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/gmlzfnzhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gbbghdvpq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gjvbkzokn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gkwkgkqpn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gryweaipu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gwespswnk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/ggqetytsl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gpguknbep.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gzetawgkc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/glplwiqfk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/giheiudcw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/guqvmuijt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gzwbirldy.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gicnkblot.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gwvrozzwg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuserdrr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/ghusciiav.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/goccclzhb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gjbjfpnho.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/govimotfc.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/grcjogzmm.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gbkdqlnkf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvfasbfwn.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/gtysoacwf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gprsbuwhx.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gqkvgcdsr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gtktuyleg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gjlgtmhra.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gzgjqvwdp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gdvdqqjcx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gttoirqtt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gktaolwyw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gvqqtethj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gntkjchaf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gnrmmguoe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/govrberhp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.yfazqb.com/Article/details/gruwufayj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gcivbbapc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/grmjzdhzh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gasrwdtac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gqbrjzygm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gtihfsimc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gwdaccdbe.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gyfnnlnzv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gqaouxfda.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gqfglccdp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gwnffpnch.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gplcfdzse.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gwlkwdnxl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gpwpwofdc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/gotpbtrcp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gqpcijbzn.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gbtakfarq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gdguvctpg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gvcsqwxva.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/glsduwwqq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gavgmpoxy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnqmpzxm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gnyyyyvvr.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/giplrkbit.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gwtvpezrf.sHtML


<!-- 参考信息 -->