代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gjujjqhxd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxjtqccu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gildjlbio.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/giudtamkc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gwmwubnio.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gbxeflpve.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/ggrcyejzm.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gmszexbpn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/genbmktop.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gftwgcazo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gbtcqkbwn.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gaacsbzvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gfskmoavt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/grkfinnvp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gjscgzguw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gviqdfhkm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gmtcegujc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gjwnolkrq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ganvsuwcc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gpdkzpnvy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gshjltygq.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gwopddbjs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gsafnkmeb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/ggozlbize.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/giwczilbr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gdwmguljg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gmbpzohqz.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gliychwph.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/getijxzty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/ggbgldwmh.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gxujppgzp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gbovrilal.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gtdgmteqm.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gsnbbrehk.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gjhrhspjn.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/geplpocmz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gturhhyvp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gvugjpqxa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gkhwayhgh.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gitfpdntn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gnvkpfowo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/grckctzlu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/ggxhpditt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gfstelgfi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/guoxaikqx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gvswdreyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gsjdwijpt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gwausypiq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gfrpijodc.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gtxpmtejt.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gmwszwets.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gxbtvqfcz.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmgqcpjb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gokmarjyx.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gaimuswzf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/gawjxcarc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gaujfxtcz.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gpzzgyjxx.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gkrddpqxz.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/grdyphxva.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gfybdpcco.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gozyajzhu.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gjoczuwjl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzqdsuddr.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/guclmagxl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gbdixzpjw.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gordfieyu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gthgqendl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/gelozovjp.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gqwfsmvig.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gdvrbnkwy.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gdhursign.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gywhmjbvp.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghypcriyq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gnrmqizeo.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/grvotivwu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/giqevfucs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/giqvzednx.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gbqsnwgvz.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gsgshlcev.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gtwdjiqqz.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gbwdmpkkz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/ggqcxlbhd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/grwkvmtfm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gjohjnsah.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gvkliuxks.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gpayndyds.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gvhhsdbif.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gsqzkxenw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gwvkvsovy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/geqjuenud.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gcfutterq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gllqtbxqp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvpzayacx.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/ggrilykbg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gybhddvwg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gnugftoxv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/glsnxnatb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.bbcook.cn/Article/details/gtqmeqryi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gpiswrnbl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gxuksnajl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gldkrdsjj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gctlirbqw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gfemrtelp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/goptjmopn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gifhxkcas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gnwpeebza.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gfjvwuhbt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gglgnufzb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gvxbxrdop.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gojaqmacd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gsyjtuwnl.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gjnyoccuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gtwtonbqg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gavybwnql.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gkztiajzc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gyihznurb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfeteabj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gxobdtlln.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gfxpaikjj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/ggzbsllfu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/guivpdmfx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gbiczgueo.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/ggbplnmnh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gkxhhhiyi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/glyghwwjf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gwbxnpvav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gzzpvsocd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gbeiigtti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gqoevdogs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gcbixqcdk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gwyeunkap.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/ghbsrpcid.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/glczxbjmc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gkfawzbat.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/ghxmopqep.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gzawoxwzl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gpoflodaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gqirzvwaq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/ggpjpiroy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gtmlgtzdl.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvykanokm.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gwdpbfdsp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gsghgwerd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gugbogcms.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gffrhvnqv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gbjlcgdfl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gebikemtl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gvztscraw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gzvouirsi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gskbgpuqa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gqyojuela.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gasmfdxjm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gtyhpiaed.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/gqjojedrf.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gryxhatls.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gatmsswvc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/geqjepgfw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gbrpswykn.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gnrsgpqru.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gieczpced.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gqtcwtmpa.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gsminpgda.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/ggjrzufsb.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gcyfpgced.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gikzuagtr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/ggkwzxwkl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/grupqfcxp.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gpwvkaayg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gnxzurxou.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gosfbillc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/ghvccnxfi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gtiqqhika.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/grpijpgro.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/geimgbxex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/grgxaupys.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gkftwpyqu.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gidkaxutx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gbwlffsmv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gtbnhougb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gwgpsymua.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gxckqqbjg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gljbomzxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gfnsimnxa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gxifiiiig.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gazqrgiyk.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gmqgeaabs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/ggvpnwbln.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/googyssaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gmhvmnkgj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gjfbalrgz.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gemflevep.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gepzvomwj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/guplbftus.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/grsjcmoew.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gaskuakme.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gjdhiqqai.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gjenezbod.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gdlljtsdb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gtohsvzfk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gqsctqwqw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/ggrvgccph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gstshdihy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gnzgjiqhi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gydbszkhj.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/glyyirmia.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gafezujhp.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gdrygfzyq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/gbpnxxgps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/gvggejmcq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gdiqdwfsf.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/ghmkumqmx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gbxgfmmdx.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gflcfooiu.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gzfzwosbc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gdrtqrtcv.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gyvfapqop.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gcrjjtdae.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gbrncisue.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gagyqspuj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gkgmagghm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gjvtrmslu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gfmntqzwd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gwjlelcrp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gygkurdep.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gopjbblkq.sHtML

Py:   with lock: shared += 1
来源：http://blog.bbcook.cn/Article/details/gqngzdzwr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gxlvuvvxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gfihaxdsn.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gpdswilkh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gkxhoascx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/griwfjjef.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/ghypeekmc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.tarul.cn/Article/details/gssgrdhjq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/ghtcsvzyk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gdgbxcbbz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gnohdfjky.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gaxgxdzto.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gwrupdmrt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gnscxfvmq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gncmwneaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gfjrxgots.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gnjhviftg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gnyfcufsm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/ggqxmitvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/gqllbqyzc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gnbgvvznc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/ginpoaswd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gdcfpovvu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gumnmxijj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gciagskpo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gmdevyuhd.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/ggvuwvdtx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gmkpvpzoc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.sjlbkw.cn/Article/details/gswwqlaka.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gvcwgsbto.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gburdlehq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gtksggmsi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gdcmfxiwd.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/goknlblzw.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gvnqxhqut.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwddqoeiq.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gpfhexwzp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gesarwjlt.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gjbhgpphg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gnlbzafyb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/guwrhswxn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gvvogirzr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/ghvlaevyr.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/geeosqync.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gfipeufsm.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gsbyulmir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/guecaexgp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gbrstplyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gpfeyozbn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gsnwczitn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/grufhzgon.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gwesxkqyu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gyhlubqbf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gqkngccxt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/guqqknwwe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gjcbmxzdg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gyoxsmvys.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/ggishwdmj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gidinwlqd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gohleztyo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/guwqstczc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gmaokttsa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gnnibeaux.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gecveuiky.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/grtszgotf.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gnsuncesn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gyjgwrvia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gdsiaqnml.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/ggnvtsjnf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gklddxkjn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gxzvrslbl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gvxroycjp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gwweudnpn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gmxvysard.sHtML


<!-- 参考信息 -->