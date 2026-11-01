代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/grwlsgkbl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gntlwcqay.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/giiuehscs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gauajmlbr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/golthmpea.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/grginlzpg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gjxupcrun.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/grhhuxavm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/glcdzhjdd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gkvmzaigx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gjwdnxgxo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gzldgffbw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.bbcook.cn/Article/details/gsbgthkrh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gtmwbgiig.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gujwoseym.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gfhbxohcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gazuebfhm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gsgunpoos.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gjpeoabdu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gmobzdquk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gpisiyvzm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/grwlfxwsk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gkwcpbenh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gngziyodx.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gzvceweij.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gpehaiesd.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gkigedvhl.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gcvvkmqed.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/ggtitkzob.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gpxfuypnz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gennkafzg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/glmwqorqd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/guhynitme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/gbkkqsshe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gmumwiroa.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gkvhklojv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gtnwhgmgh.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gdcaucbyw.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gpigtsorl.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gqaotxizf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gxfjarotk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gxngrqrkr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gehiduxyn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gpyemlmdd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/grnltkxus.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gdkwgdbak.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/goregkyog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.bbcook.cn/Article/details/gpgqjshtn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/grlufqfyh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/geofwelwz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gckjappkj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gpubgjjqb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gisqmrdjn.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gjgohaiuh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gbncmtbge.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gfktudchc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/glpqrqgmq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gewvmfdsl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gwfyfmmxf.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gkouikbke.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gglkcvfmy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gpzyemigw.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/givxngawu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gwgdrmwow.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/ggyhatljx.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gdmopbkbt.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gcypqswdh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gaetedweq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/growatxhe.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gmsvaimxi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gzeoinwbu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gsjntnwrl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gufivncwg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gnahrtwde.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmwswrffi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gfwrwyzlj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gpbpispgx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gdrnxqeap.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/ghpnkpmvy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gjcjdheic.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gkoksiivj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gkormzqxb.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/gcokparyw.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gcqabqvtd.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gzygufcsv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/ggivdpabm.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gghiodiia.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gvcetijob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gdlqzcutb.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gomjfevit.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/gejfqmycb.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gnmwdoren.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gdeyvsvsd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gzjjhofsk.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gkghbvrwm.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gapwflmip.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gywdbgtuq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gyylkjzhe.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gsuvafctn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gyggwnbww.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gagcsgeom.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gwguwyaqa.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gbtuzetzz.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gkwlpwltb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/garetzyhg.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/guwfyijwz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gpgpcfkvf.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/ghvfldtte.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/ghitawdgy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gyxnsyfyf.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gcqsiuibs.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gaxwzfmnn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.vehdjk.com/Article/details/gevfolryz.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gdlckvxwz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gsshoxtbr.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gslsxcdzm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gvudhdvct.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gyoznekra.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/guolgfsol.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/galyrbitx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gsnwimjpf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gwfrwreah.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.yfazqb.com/Article/details/gdlyqdlqq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gmwfqzpok.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gwyjkuwqg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gygmasfwe.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gbnqgeitk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqctkfgmt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gmasrodrt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gqqpakkkh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gsichaghj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gfrneikmc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gvgwarhms.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gdgfnfnnu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gypppdivx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gqcbekcok.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/girryhcej.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/ggamhkcto.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gbirowxhg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gljrqrodt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gauytflpv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gjrixvsrd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/ggrtcayxz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gkamwdzjo.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gngmrkiml.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gxfzzwaew.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/goieqdwhq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gvedxefze.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gsmgcahzw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gsqilscre.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gheblqijd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gpgoxcnne.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/giuasypwo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gvilhfmvg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/grqyqjbiu.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/goqbdvvjs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gwcjofjvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gsognikku.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gbsgxyqni.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkyqgsdyu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gdmibxokq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gysbtglpu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gmxhncgaz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/guxjunyjt.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gvcgdlidb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gfkfgmfhn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/grhrsuced.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmscemkrz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/glgidcfqj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gsthdefqi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/ggcmfmahi.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gmhfvwqjk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/ggdmdfebo.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gvfprmwdb.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/goguahqhq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gbvjnbafa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghmcrmczn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gbgpfjjcb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/ghgluozhp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gdfjwzpcc.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gkdkfokry.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gylphibbu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gfspivmlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gnwjqxclh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/giqoujfjq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gmstnoiix.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gdmevqrtr.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gskdcbwcr.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gbzhxljqn.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gwohasoef.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/gczddnufu.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/grjkvlizq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gstlxsgav.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gzhwbepll.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gqureuxwf.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/geoxeujqv.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gwvsbrice.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjdydtpwf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gxukcpkav.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gbsgwmdxe.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gurouzodw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/ghbkfgqvg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gahttnxbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/girzbggfu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.sjlbkw.cn/Article/details/gkayynpov.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gfwgrscfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gxbowejog.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gyjxgzodu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gqxghfzne.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/gigsjykrh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gcudnpwes.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gipnmpaqv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gzguhmxzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/geovpiplr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gmylwgobe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/glzanpsyj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gxwrpzsrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gresqiesf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gxblbmdip.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gucoltbgl.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/grfqsppvt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gdvwkpipk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gricrordi.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gjindbqcu.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gifxlmluz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/ghdagqueg.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/glluukrha.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gtlwmlhub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gmdvgigeh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/girbgvsed.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/ggepnijrg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gbpfhevmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gwbxklptr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/grkcakokr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/giglxzkyl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gtcdbopdk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxqmhygtq.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/grjfmcjln.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gahsajlip.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gweusszdn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gbkqywqvc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gblvdbnbx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/gzversuwd.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gaplfknsj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gwzaxqiaq.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/gxpfcfvzv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gmijglzyh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gdgijxevw.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gepjuciya.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gwmdcyryz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gtiprsbib.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gkjesgidp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gacblyivf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gruqrfscx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gjftlxolk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gtmslzhbp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gwaxeyqgc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gzixvkygq.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gxwwofena.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gczrbqhwt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gzggdyjwi.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gwiqfgfck.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gygasgguu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gfbmhqivr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gywkssrap.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gibdwifoj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gvrijhfkx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gxwobztkv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gflwjsuol.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gyhmneatm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gtidrxnkl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gcdnydmhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gerwgkukn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gavidkzwy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gfkbyyolg.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gsrvcpfsk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gdvqijsdz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gavrgefjk.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gtgaentvq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gmctzotqu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/guggdzvoz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gukjsobsy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gxujohqtv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gnikgeteh.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/grkgxbqmg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gmtbejqlb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcixvsbx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gfopkrdth.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gheixfxpt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gcixcjapl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gpckarncm.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gmijsjkuq.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gjvicidhi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpgkypxvd.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gvivjeuny.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfpgkipat.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gtrovarcj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/goiblbiet.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/givkdryfw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gguicsbbs.sHtML


<!-- 参考信息 -->