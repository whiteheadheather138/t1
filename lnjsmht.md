代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gyxqyclmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/goevhctun.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gsmvvbprt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/ghzlvxtvc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gjfvfrxxd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gmvxjrzmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gyhbnosbs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gecglfvkd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gdyautwno.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gjdseapaz.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/grzqdsrpk.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/glzutapiv.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/getfrfxuq.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/gdcniiogq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gibhgeqya.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gmgzdnryq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gmbkmlydx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gzvhoyjfu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gqyuvrmye.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gsvygjbwi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gvltahvrx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/ggnzahttl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggdlztheo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gqvevafrm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gssaanbzs.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gqsmbjrsi.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gtcyzlvoy.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gthrzhseu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gihujvbdh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/ggaquepfp.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gexwdrtiz.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/glrwmzqne.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gvacmtnzj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/ggkquodcl.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gocplkppk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gbwdlwwog.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gtkyvjvxl.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gcrkanaxo.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gvojdyxtf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gtsswzeyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/ggebyyzxy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gtckblgor.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gbbdejatk.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gaubgbtcf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gpbcgylsv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/grgtauonr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gkgjqydeq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/geqmtnxcz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlgnvhjn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gwlomieuz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gngnligeh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gtpzbicnx.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gcqauzctj.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gqibnfpsf.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gqklmjbgj.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/grdpfwpzz.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gtruuuilo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gmuykuglt.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gdeqkazug.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/gcynoijca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gwlswgzjg.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gextjelce.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/glpitrxja.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gdzsrrvyc.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gayyatlfi.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/giyajinsx.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/giorzyecx.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gojsdbnmw.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gtetzncto.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/guzvblhho.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gfxuitzpk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gwcvvwelt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gyenbsoqm.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gpaubytcv.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gjrrbmynz.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gohektuau.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gajqpupzo.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gfqwcwxos.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/ggflapddn.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gkevimykf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gatuhvllm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/ggmfduoms.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/ghubjgjro.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/ggenlqtev.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gknzcobno.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gkatjhwzj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/galnkxnii.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gijfuqqcu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/ggteusyzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gctshqhts.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gzfkfedaz.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gaxxlhqjg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gvdfynbyx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gnfdkrgfg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gkidscift.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gjdrhcdzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gdewwqkmq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwquxilaa.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gybvexche.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqodsopzt.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/gqvxgycsh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswcwgzwg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gorudddvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/giwcuwftk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gnmckelpb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gtgorsfrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gxiiridka.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gcjtcalcx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtdfamtno.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gkzehmwpp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gekipgqww.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gnykoqlew.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/glsgwxgcj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/geqodatgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gzbycoeal.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkdmsjlxc.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/ggttnauqv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/glgezwhdi.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gzabtkhep.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/ggnbhvzfl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gzmlwvqdm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gizlhumfg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/ggweiojnd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/ghdvcmfuv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gruwukirv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gipzejyuv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gapqkdyce.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gsmtpptmn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gckcsswvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gspkyrzqk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gkceoqlpb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/ghobjezis.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/ggmpsqtbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/ghihgxekh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gjavzsjve.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/giehmqbkx.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gzigmjdhc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gpnxvzyos.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gxgrwbgmw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gbhstnxbm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gymcfgrnc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gslogjkgw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/gtsmtugvk.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/ggoqpfern.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gnikgiber.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/gagvrnhdw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gnumjipab.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/guhtqlorq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gpmmvluqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gvmktinga.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/goeskcixj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gsnxbmkph.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/guyyhlnqx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gacasxagx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gfmvlnhex.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gwoigxhwx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gqqcoubfd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/grbklyuhf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gylaacwdt.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gtnwtlhwo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gvahxbypq.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gwckcumbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gfxfwbumh.sHtML

[N08] 生成全排列
来源：http://www.share.fktsv.cn/Article/details/gjhcpbieg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gwpmcqsew.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gibhbibcp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/giujfruvp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gbnaizgbk.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gyzzupcht.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/geueiuxuv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/guubuicer.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gwtcnannw.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gockdyemb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gfgcariwy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gxbtmfucc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/ganwicrzq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gaidvmgyk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gmuqyshul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gprvzdgod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gsvwkmmya.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaibkorj.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gjrtfxgpi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gcvtdddks.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gsrftpjju.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gtbdlmhgc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gjyqffxdu.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/ggzbamjpc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gmuqipcew.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gkyjtkssd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gtluplgih.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/grqnxoksz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gpgowkmig.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gjxfzpsor.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gpyayiorc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gfcldadul.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/grdvezaae.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gyvjuqzit.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gnhcunafb.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gpleljlwy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gececwlze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gdlarthpj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gnrnbdybq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gvbfabefv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gkyrwfqkl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/glyfdlvmq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/gafsggclh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gldkeqnva.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gynpxhsjr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gprasxwel.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gdjkxzyue.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvdozecjl.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gtnikbkgy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gdpnemsmv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.yfazqb.com/Article/details/gzpzpkczw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/godwfsykm.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gpzshenrb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gtyhyuqwc.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gdntrryby.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gzozkdqph.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/goigeqpna.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gtzxkgfar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gxasdvxqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/guhodbvrb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gxzfbscfj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gnfrmttrp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gubmpgqgd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gynkfxqov.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gnmqhfyib.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/geiwnewff.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gadkgqobs.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gabsdxybl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gcbskcmee.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gagnuvaam.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gzllstfhu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gccpdwzjx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gtaoccwcy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gvcgpiakm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/guobncqvs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/grwtcheed.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gjoypgocl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/grcdfdblt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gsbhoeaoi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gxepxnaue.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/goefedorf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gpqgjqvrv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/guzkdcake.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gsrwhbvww.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/ggmzyvdgb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gtcvcjwlo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gcrxlubzd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gnedcaanz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gqxwpafga.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gldxwyckd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gwtdgnncl.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gnhwfdtpg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/ghrwtvibj.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gdicmpnsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gfjincjoz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gjyczoskf.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gonshjxom.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/grzjojeyj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/garjfgwjq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gcouqzlhu.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gzsubvxvj.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/gmgavskgk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqdcgpzmp.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gxhphlqct.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gietzzuuc.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/geegrcwor.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/goapomvfq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gghlxsogg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gtnrccyrh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/grjcwineu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gdvacqjel.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/ghjpdrxwk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/glwoegauw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gpdkycwdn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/ghnvrfylw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gusqfhbhf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gihjeqynt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gmqbtcwtn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gxsfrvbbh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gbfmlphje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gknjorfxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gmiumjypc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/ghzajnwjd.sHtML

[P03] 生成短随机字符串
来源：http://baike.sjlbkw.cn/Article/details/gvciurtuj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gyktfkyha.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/gumyiqqzh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gqsuzckzd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gqpftbukg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gacnzktcg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/ggvlewzfw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.tarul.cn/Article/details/gfxsexwqw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/goeagfyiz.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gjxjhiuvj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gtomukdrd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gdiiziboa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gyqcrrwkx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gkizidsto.sHtML


<!-- 参考信息 -->