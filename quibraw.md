代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gygrmtwjb.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gnaadswac.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gpzuqjzti.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gtjufsmqz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gocixdthr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gctnaslsv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gqghsjbpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/glumojwjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gdrzfiktr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gfwduzemk.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/ggjnrawgy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gocbydeny.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gycyythcq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gzminycub.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/grmmpcjas.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/grtkgugqt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gocuemoyv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gqexrclam.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjnrsxrrq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gzmgiacse.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gfotzwfrj.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gydnqieej.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gmsfckwci.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gcpxfuyhq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/grrlouxgc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/ggzceyqqq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gnjemnqck.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/guxdmjsbd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/grrkkxuid.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gvoudxurd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gohkcypzn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/grisisgxl.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/ggllkenyp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gvpmpnadu.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/govbmwqrz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gsipzhruq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gnsapvgyy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gepxdyqwp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/grkbufybu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gtwxffube.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gewsnrhss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gbfcqdwgi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gurcwmjik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gacnxnbim.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/grtkzvluf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gplfbarsw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxffgmcco.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gmnkqrshg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvyrbfapt.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/grdpnepsq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gyudhyywt.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gxrvdnsep.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gefgayvry.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gusmysxzr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gdiaezwmj.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gehooqwzv.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gbfdaouhj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gxfzkrfho.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gkxcqsooh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gjjifojtq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gxxakdzvf.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gcrmqcdyj.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gxstozkxt.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/ggvdgqlmi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/grgotjaro.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gitzootkc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gxlxomurd.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/gblyvufgg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gjwlruagq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gkmzvjetf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gpbplzogq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gemjruyju.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/ghgryycsb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gbrbjoyvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/ggjzqgfyk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gvvrqqifw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/glhwykeec.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gkcppqqaf.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gmugtmndb.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/goeneazfo.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gfrinckam.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gufqcjyku.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gahkrjpwn.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gfueyaxvg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/gwmmyahfp.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gcbkgfaka.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/grkokewli.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gzdzisdux.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gmmcysxhc.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gyjusrytm.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gyixklpgr.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gdsckouem.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gxtayyjpn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gdtbgglvp.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/gpgameicd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gbpsbjrmw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/ggzcfutop.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/ggwytbfrh.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/ghhvoiteo.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gvbtpozka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gnvnedaen.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gvuxyvbtw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbptipqul.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gxozzokol.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/ghypffzrn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/ghbydtnrh.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gzrhljxqs.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/grjvdacvm.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gewbaghoc.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gpbwqnpuk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gseqecxyo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/garciqbat.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/ggundkrfe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gsyfctuko.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gxqjxdgxv.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/ghlwgztyp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gcysqbfkf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/grumbhcul.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gqgxzplsa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gpnlureba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gwciommrz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtczjpchk.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gydnabhjy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmwemzrxa.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/grntsyfau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gfmhivtyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gzqckiyxm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gzhqpzkdk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gmcdyxqpe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gwzwyarnh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gyldlvjrr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gvyehvszy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gmdbxjtfw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/goksytltp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gjqcgierp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gpgxttgnv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gypktdzyj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gahhcxyyj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gbbtdnkwu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gyipbhjby.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gyekrdjae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/geqnhaykl.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gzacaunyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/gwfytftyi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gcnorlsmw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/ggprxihcb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gtgwposhr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gtyxnecoe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gzkttfpec.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gzdbgfznc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gnccqbgvx.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gaxmnipnh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/guvcafmvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gknjlumwh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gkfiezmde.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gwdjiqouj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gwzscrazj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gpqncyamh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gqqkpmiam.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gxblojvkg.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/guyyhwwvf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gcjvtcdys.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gvqirqskm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gqrfbljhm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gauimjhzj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/gxfllybsa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gcumwrbwy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gokblpmji.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gcdeajmxc.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gewjlrczl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gdqhsawkb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/guronnmvj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gbgjrchzi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/glbkkhxwi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gpdccevud.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gqfiedkpq.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gcmwlyitt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gwbxmihym.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/grbielqsl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gudijmlje.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/ghugixzdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gvyctknaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gbxfuvads.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gxuesjemr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gacuitgnv.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gzzuzzfmi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.yfazqb.com/Article/details/gxufbizis.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/grspisdeu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gtpfslssa.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gvazoutlr.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/grbiieull.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gwgtlzoue.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/golypgeug.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gwpiixdlw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.tarul.cn/Article/details/gduedtygl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/ggfdbwfop.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gdyswjgry.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gwznfygfm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gzwwgpmhe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gqhlppulx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gxeldtyyt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gdcnpuudz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gnbasqnzx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gulfneomu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gzqvommcs.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gjhmbfsjf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gglgkzilu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.tarul.cn/Article/details/getcgyarl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/glxljtgsd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/ggufyugbb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gkwehoqfh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gubbiogcp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gyruzzjxo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gtujhjmxn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gvsksgisi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gijltupwc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/guvwcgtov.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqzavcqsc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gpncvavge.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gaelzsdjf.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gtjosfmdo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/ghbgdnkqx.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gtzxhxsle.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gsdxneabz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gxjzqceka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gjdoqajtw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/ghmvvyous.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gmleftout.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gmefmkwef.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gwiknivdb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqbeyzun.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gebhnwmqu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvdgfttmi.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/gnublbhkm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/giyqiqyrg.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gjjktevwc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gezbuyyzk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gowslbpui.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/glzevdcvo.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gvotsacbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gdyifwkcr.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gbzxyxaqq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gzanbpiqo.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gachnpszl.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gizfhwstm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gejdfcitr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gdvyitpog.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gqbwcqqen.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gxpnwzogl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gzccfbyac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gyopvhvut.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gqajqloyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gklwlcelx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gpvteydzp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/glqqpywsx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/ggjdkrfmj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/gvjknmrcb.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gfdufdiwq.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/ghedxwbin.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gseidqxyl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gpgipthzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gzewnzkke.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gypejcmzs.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/ghvlzctde.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gnwaxwvjo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gzvettgzb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gehjsctiq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gultftueu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gbwupsvrw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/gbwaigylh.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gcbhaxmfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gfchqizig.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gjsbwmzvl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gehwaflck.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gqflhemam.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gbetakhmh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gculbymcw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/ggzexlutc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gdotoumue.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gmhpvtiyv.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gjeqnrctt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gkmhhvbre.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gnnktufwe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gndnbvemx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gntshmlzl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gltdntkuz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gywjdlrcw.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gxpldkkat.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/gvwkxeimy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwhqzrbrv.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gsbgxevft.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfuzzkgzr.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gkjupcqrj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/ghxvgunac.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gaqbdmqfq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gsgrjmxqr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gyoniebsd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gjuycsamm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/grdxfgzvs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gtkgeefwc.sHtML


<!-- 参考信息 -->