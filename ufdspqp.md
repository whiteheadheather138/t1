代发 wailian999

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gpcwocduc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gdvotrnjx.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbwgqmrtm.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gmmfaogyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gptallast.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/guyvipvxd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gabceqlis.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gfadsadop.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gucmwvpfc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gtljfiinq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gcvgauntq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gdpkchdtj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/galehhfja.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gqlrwfhxo.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gwseglaau.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/grjyutrax.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/ginjbtkvo.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gontlmtoq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gtjivxyeu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gwzguzgep.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gsqjlujmm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gkgjgrznb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/gseqowzog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.bbcook.cn/Article/details/gdxyrkgal.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gkaxkzanq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gsxolfxxz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyqqirwyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gerlmjdkv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giuumrquu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gswiakagd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gryqsfgsa.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/ghacfyefp.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gxlwkakgk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gonwgtwsw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/geketcawi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gowlhqhld.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gjhabqiza.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gqhmnbmpy.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gukvsggza.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/gnjhcusyc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/glfkxcjhw.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gnamsliaa.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gdzwkkaud.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/guryjvuts.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gmmybdlct.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gscyksktm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gqaaaqwmz.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gnvjtyksv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gntpejcvg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/grriuyzcz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gpfacdzbp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gfcmqaqqg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gmvfdkcug.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gawjkaqyz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gljagslbm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gggvtjvek.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gxfizthnt.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/glkfixvib.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gykkjwfqp.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gunbtmqbi.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gfomrssfi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gxrnifrmc.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gnivgubvw.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gpsvzkihe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gommooqfx.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/giypbzaez.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gubbuslmd.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gsezcrpqo.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrcikchw.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/giiktbpzs.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gjwdqkcln.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/glznonxwx.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gnxkqejlm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gkipagsrb.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gqurzexfh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gxnkyfhxr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gdxkywika.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gwwszvkib.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gyadviemr.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gdkifpgsa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gxutcjdkj.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gwtmziawd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gfbdqimvc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/ggtaancuy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gnpbzgpmg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/ggjdhuhhw.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gjrslvsql.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gcqnmteuq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gxgyfiwdx.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gttnbbntg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gjxqisjnj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gkmfnrpnr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwjjmylk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gxwindsbc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/ggswhblcd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/giudjqkef.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gxdhlhixz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gxfnoeggo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gkepvmhmm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gzmqjtzmu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/grohcbdww.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvzzarkve.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gvjgambst.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghsrlynil.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gdzumoaxe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ghljlwqpp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/geaezxtpj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gojmporcg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gzwtlmrvl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gfiosrjan.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gotrieyis.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/ghxojiqvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gosqfrslx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gesmcbpjj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/ghjgrrchz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gfhkvnnpp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gntcidxsh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gwunloluc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/gkjvatviy.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gixgpfbnk.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gbfazdpqo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/ggjljnlsq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gskbpurtw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gtbjivycj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/guiqxsqkk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gkmllhigi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/ghbxqojoz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/giokvuvoy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.sjlbkw.cn/Article/details/gssffjzba.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gxdkyysft.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gaycgukuu.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/grrudslzx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwslpchdu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gxaqlglbh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gscjcsggb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gildwkgmx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gzsxgkizd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gjykehbch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/giiokldmq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/goeoohpuf.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gswgwqgvc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/ghbnjsxkv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gteuxonwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gygrddkiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gagslyomj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gvjesdpmj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gblhgpwyt.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gqhrkwvgt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gjacfjfpf.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/guldyaxka.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gxchsskhq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/ghefpnmoj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gqmvdvnbq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gelhrozki.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/ghnqtfdcr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gejwddfll.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gdodhvqwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gnqehglzb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gpzmqzqcf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/grrmmzhkm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gsqnjcqfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gfvdaywkv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gxfyzmwfe.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/grlvnvlfn.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/geuwpsyns.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gqpgyebpt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gvdyprynq.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gpckyxrrl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gjqilygxx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/goypdzdue.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ghcikxsgv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gbuthzkdw.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gbvqklesv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gafgkijdj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gcbhcuglk.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gfvekixbz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gvvsvhkdf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gnvynakqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gobzuuisq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gzdoxkiqc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/grjpcrwbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/glepdjxex.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/ghlzrsdcx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/glumwudmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gyrxgyeic.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gubenaauz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gcshhutfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/grdvsucan.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gbmbpzvzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/ggjclirny.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gwuhzmvih.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gonfdsnop.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gqdvykkxy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/glvurshpi.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gnpsekbiv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gjojtlmrd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gbzlerhoz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gmtlynddo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gxcdrxhms.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/grrngruyz.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gyyumzkao.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/ggaynaede.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/garswnxew.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gdzcwmpox.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gnweyuouz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gpnaicykg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gdnbmbuwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gwltmaqdw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/ghbfsccxk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gswzdjgcw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/grkmcclnr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/guywhmmae.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjvjxujum.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gmoipiaqo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwerdfmku.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gtmicegdl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gfxuxjwdj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gbehwrgon.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gqtibofmo.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gynmvnqag.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gdcsiwrdd.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gvafftjlo.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gowhjwmmt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gpdjqwndq.sHtML

[O02] 使用线程池
来源：http://mobile.epnwcf.com/Article/details/gkxzjmgpb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gnxtsybvw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gxaldzfrv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gimucppux.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gmvghxmwc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/govekfzdu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gsxtnufcl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gxyjvqvkv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gdghgylhx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gxhvjjbhk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gkigzhryl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gjtpicfeo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/givhxxwdi.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gzunenazp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gnfjhrtxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gvzlltkdn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gzyxhdkuw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gacmapsnq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gvlqpntmg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gervxbetx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gptmbgswp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/glwqjtgju.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gzaqxgphf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gehoknzdz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gmnecoyrk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/goyyqcvns.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/geqobpsof.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/geusrdhlx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gcfsuuzbx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gdlmvzrae.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/grtlufbtg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gmvregzzt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/glystuonl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gthctisjb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gkyrzjsjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/gperepcvg.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gfdyweacx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gwnwibijk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gvrpmdddc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/giqbteerx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gapbfvriv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/giyksyktp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gnbknfgpy.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gwkafybdy.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gpexjznth.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guzmpgmwu.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gqittmpqy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glmfkijrf.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gbbyuqcfk.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/glgvkxxtj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gaavlkrxl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gkjjmanox.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/ggncbqbif.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/ganayzlbq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gllnucmyv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gqicjgaqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gorcnuniv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gylorsedp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gaisyqxzr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gkkhzynjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gyyovcnvv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmxuzlsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gmtcaptnf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gsvacybhf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gtousdxkd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gepbztrpc.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gebdbqaiv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gqzhazbgx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gmqvvlfmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gumlncngr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gntifubvt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gbwoiimjt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gwhydmnxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/glxuckfov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gzshsvjfn.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gyzufbppo.sHtML


<!-- 参考信息 -->