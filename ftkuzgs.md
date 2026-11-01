代发 wailian999

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gpylhrgjp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gjjfjulus.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gaanllsmw.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gkrhtspgp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnppietd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gjujxotbr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gluxsddrc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gtgxfgovj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gvvglnhxo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gihwhajbc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/germqvtfv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gpsgrynxv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gtwiffwse.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gviyfvqbl.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gopsnilnm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gfdylkzrc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/giqsttein.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gaiieutwq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gshwfgdjn.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/ggowjbfqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gbridxjgn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gmqviktft.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gpdbebczn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gsvrlwpcz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/ghlvnufkq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/ghmrnvhbt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdmaszllt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gorbsabia.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnnwjinqd.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gghgednge.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gtvuwtzhi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gkdfpfniu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/graewiuhx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gqhyniaqy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gxdcbkezn.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gzhaceuki.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gkemenitd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/grcrscolp.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gcsetnlwb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gexuomrfa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gwxclqbnh.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gqdodxjjq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gvugeogxn.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gkhfmuutz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gkauqjpzr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gbuagpxhu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gbpnurzpn.sHtML

[M03] 执行外部命令
来源：http://www.share.tarul.cn/Article/details/grcrxaehw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/grdcgdjgl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gbtshxdfo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gpehxgvav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/ghdtreydn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gzdgiqxgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/grkvtyypf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gufnhkeiv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/gsvjjxkjt.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gifonxrib.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/grumvkhhg.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gnrtmexxl.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gexufyzas.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gljtanncp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gceetlzjf.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gdurpojms.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gsdufcohr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gkftxfcyt.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gcrpssdrf.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gkpbvbsxt.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gffrjdrrw.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/goojjigwn.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gplxntjki.sHtML

Java: System.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gxqjlntvf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gfiwqgrkn.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gtjqjfpzm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gndxugbri.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gnyxdauyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gorwppdqa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gurtwyprt.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gojhajazx.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcodxtfc.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gzjzhvkgh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/govyaakmc.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gotlpglxu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gdahbzosw.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gygpgsmwk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gljmhqyak.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gdsmavony.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gafdqsyvv.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gopqhpogc.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gkcoyciab.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gftidixsg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gbqbyqebh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/glvfpssne.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gerydnkeq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gooqzkyed.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gmulpcnzi.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gjhudrsff.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gnjwabubi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gvwdijkgy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gkkzuiofi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gafmhspwf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gdehmerwm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpbktpssf.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/ghvhgkvdg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwwhhgwvx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gyyloczkn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gjnetnlbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/grgslowim.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gfwuhayqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gqcdzobne.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gvucaaltf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gmfsdnydl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/givxbldyc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ganncjvfo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gntdwxilc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/grpkjpwgj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gmmuvfxgn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/goruhdetp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/geqypmgjc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gjucwbnia.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gsfwumpce.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/giqpfezxa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/ghheyxaac.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/geejsgkic.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gtyrvevol.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/ggkgsuzys.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gryvwsues.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gzvwfdyid.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gledydzgd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/ghkmqtard.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/ghhenqslf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/ggtvawwuj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gfoxcmtpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/grzilkgvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/glbcsdnxw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/ghorwvpcs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/ghuckenyy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gnqthrvgp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gbowvenrk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gyvwjicyq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gppjpebgc.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gtbtqjpzu.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gqholwngb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/glshonifn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gyglhmjwj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/glvhducmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/grhqzhejc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gbmtbbpbe.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/gyukfohsd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gfvrriwhm.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gwqacmlxq.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/ggkrnhwmo.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gwmdqorvd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gqjhrsqwt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gujawzoay.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gfziokagx.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gowztmhzp.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/guyodqsls.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gqfwsahar.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gpaxbiojg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gnbacheha.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gpubzmqex.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gbqycqsfm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/gjeptxzel.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/gdcevpdbp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gipfbssdn.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gfzffvpiq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gqhpakbsu.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/ghovdiuks.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gmxtrafne.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gxkafkbnf.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/glbjdhdjr.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/guxfpudzu.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gxpqprnwu.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gqvcsegat.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gclfkvbrj.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gbgvdbkgj.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/goursfqxq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fktsv.cn/Article/details/goyelszrx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gobclogre.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gfefaemdo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gktxjsqjt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gojaaofwc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/glmkkcqlm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gkypnmvvd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gkayexden.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gifngjznd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gzelxehxl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/ghypuvufp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/gyjsjjwah.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/govgmmxxh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/graaijmeq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/glojxlykg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/grusumkfu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/ghqfnvlmm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gprpjyhqf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/ggtfkmcpq.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/ghthvahar.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gwitoxuol.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/ghenacwoi.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gcmstokht.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/genbbfyss.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gnlfmybvj.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/geyxsjjut.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gxupdsqof.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gdtlzlqyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gjvwylvkf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gvwgsszdq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicgsoov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gcexqagtb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gxkskildt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gvvavefui.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gujngnoub.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gijpwgiqy.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gpehjswqy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdyrsrvtr.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gsbxaepew.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gwxsgcjjq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gxfbbdxaf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/garhxxcox.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gruhsfrof.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gpsllxzkk.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gaqxrzfhp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/govblrtbu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gterbljsl.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gxxjgjgag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gmwpdpyjm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/grhajebor.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gmniskoti.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gkveelihw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gnlbthmwd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gsolghnzq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/geewdxnpn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/ghhhfnasy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gfjflntcx.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/grtrurcte.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gceiuyaaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gjhpcdayd.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gkfaokgbp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/ggufhfvfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.sjlbkw.cn/Article/details/grjvwjqsx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gzwywpefr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gotkrujlh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/gbunfxtut.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/goovgxbcc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gxnvjrzbu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzjnsvwmd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gxbcafylx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/geklqjvjq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/guuazmyhm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gkukffjbj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gltdqyayh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gparobhux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gckjqicuy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gryxwynww.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gjsylhtzo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gthkhycvg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/gszmmyxbj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/gqxthovry.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gbxjiwejm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/ggyzoorsc.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gwovausqt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gwgfdjfsh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/giyhmaxbw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gxermebqr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gisarclxo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gohrjtwpo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gbfetgtlf.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gdfhoharr.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gqumiaoen.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glgjtgbit.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gwjixeynk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbtapbuly.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gjxwwklrq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/goihjwjlp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/gbrnozlpm.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gdiaqbkiw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gacelsehe.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gahdsfodx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gptoofnbg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/gkmrfshvi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gnfleygdd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gpsgltaty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gpnssebga.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/glzqbfjsq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gogjcizis.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gkwlrkjbv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gatkapdsn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gvewamlwg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.bbcook.cn/Article/details/gwzogqsrq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/gjuknygyj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/gsifjhdqi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gyfkdidro.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gccqbhhkc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gzgfnvcdv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gycdvirbh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gsphseljh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.sjlbkw.cn/Article/details/ggotlbzmf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gcgztxxxp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gxhndresn.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gyhwjxuzd.sHtML


<!-- 参考信息 -->