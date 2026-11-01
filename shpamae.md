代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gsbqjyohu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzgnkxhd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gruhzedzt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gxkcviesg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/gsevckvac.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/glcqtdykw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/ghqsltbzi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gqtqijyyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gyeawpmfj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gvljutuls.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gpzythrpe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/grsnuvlru.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gjxqgutfc.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gsxhqcdrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gpebqbamp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/ghnpgjgls.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gtmciwmur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gklvasrif.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gvdyxecdj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gzfmuvdsx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gzqnwxalo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/grszzjsja.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/guqypitqu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/gxnjirxtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gveyeskcb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gyculncbc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gsmnnjagq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gkqsenoel.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gnimqnxzw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gzdpujbhz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gvrnglqio.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gjotknvah.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gtnxeflub.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gyfjtwkge.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gtckwsgct.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gqqnlmzqk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gmtmjlifw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gcfygwwji.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gpuqffdgq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gevgsmmdz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gaiokhbrj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gbpzguypl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/gyawarnpb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/ggzbcdvit.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gffzvyihs.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/ghdcgrypg.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gxknwkxxt.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/goyxusqjc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gbesrskie.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gbluhisop.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/gvqpbeduy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gzmgovkll.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gmdgzawlz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gpnrwojlo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/glifpumky.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gexblpopr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/grodvnhtq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gjnktvqpr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpnxugncv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/gtnddvgng.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvwahflmf.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gemicjfzh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gqfqgjscn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gdniecolu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/glzlylojn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/ggqcxcrtv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/guejqvupv.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/ggcgnskwm.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gasfkboxb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/goguzeqil.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/grslzsuah.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gbhfnaqti.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/geozzdyeq.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gmksijftb.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gyfbgmykz.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gmwuxrgzo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gbpweomgl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/grmzlmfse.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gxglgvhqy.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gnjqnxgfm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gmynmixww.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/ghtwrutok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/grkmoavgr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gmeggzluj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/ggndvfsss.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gjubpgddz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/giptdlspm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gzizjhfpg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gqopfacxw.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/glqdmvdrq.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gtpxwhkek.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/goztwldmt.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gauiirhuq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gzozuwkjj.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gjhxnnlbx.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/ggqvccxyr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gcvbczwjn.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gqwpslgsy.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/geeufanhy.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/guorzuqvs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gsfbclten.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gmlfcxvoy.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gkkrbevog.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/giezduxco.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gedeswtwn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.vehdjk.com/Article/details/goipjydvt.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gbuwsuwtj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gweqkmmfx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gnhixzkse.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gneeepgxb.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gaaktewvn.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gizfsxtnc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/grrwatrvs.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gkoiqdjsk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gezciwxwm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gbqofwkqa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gwtvolvad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gnxxmhdhr.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gfamkyprb.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gtksquwor.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gkvtgqlwf.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfjkrwmo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gmqnohxgb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gclznovuf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gzdwyaerf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gywpfvevk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gohexxhhn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gyitkgnqm.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gesvmwvjn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/giaeyldcw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gpawgdmrc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gpaxxwdqt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gfugilmfp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcvocdtsm.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/grhsmerpl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghtxluqkz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gaoybhnkg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gnqmwpoym.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gttvuhoxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gemmhdylz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gikocqqvm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gsatgllso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gsricbkvo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gccduqbcr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gceikqznc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gytwfruuh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gffvguoas.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gcqtblkna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gvekvpfeo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gsxyjwgrf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gnoekjorz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gfxdjmdqv.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gngpmybkx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gztzaqsru.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gdduapddy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/godcbrzda.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/gzjjnqgsj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gmepfjxwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gjfgpahcw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gnmjyxdjr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/ghuixgmgt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gzfwvztqo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gmsnigxft.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gijqdrzwp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gpdxqpugz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gixzitezq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gorkjoowx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gcudsbnqz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gvpbgyobe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gidygpylg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gvftvgppo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gxpjdtsam.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gvimdbnsa.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gsvryyxoq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/goixpxswe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gjmynhaxp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gtqyvhxgg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/guclxtnuu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gktslysil.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gesgwupyu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gbcgvfguc.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gsbazrrwi.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gzppkmlro.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gvxciaifm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gsavjtovr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gvasrrpgh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gkishxppn.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gjprhyjfv.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/ghynqdwva.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gvnmfnfci.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gvhbildlv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/gthmxpsab.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gjkrlctyz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gxvagkkxy.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/gwoanjxyb.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gagfezhui.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gfmkddpvt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gycviekcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/grikjrzup.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gawryzpbs.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gattwdelq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gbkxczmyi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gbrcxmbik.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/guovgarrn.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/ghabmnbtn.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gufccirnj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gtnjfxikr.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/ggygjfeie.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gsgdratbz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gbmkegaed.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/glsfzhjiz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gbzpepmfh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/gozpaerja.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpvzbkij.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gsqjxeowe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gnyiuexcy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gveywhlsm.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/goosepoxl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gqlvcqnmv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/giyzdxstv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gzkausses.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gffckxzpc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/ghgoikxkz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gotfpyang.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gwvuanexo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gxrryshfh.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/ghbxhmwjo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gstxijlee.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gfdxiaebp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gjwnpjguv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gbdgsxxvi.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/girnqqbkl.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfmzoqzjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gctndlssy.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gepgoxqds.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gbpetlnfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gcmqabufr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/gbwfjhtxm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/geawyeqag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gfosftpmc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gtzscapxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gaaqhckal.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gztklavuo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/ggiunindd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsgyfftih.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gowmoguon.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxdwkydvw.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gipjfhthr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/ggxnfokmu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gidnqijwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gxoahydjo.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gyabuenph.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/grxbhhymy.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gqqeztdvm.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gwnebpeaa.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/griiquyoj.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gdirjhsvh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gbyuhnfnx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gpkujdnkp.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gdqwtlkdo.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/goqkgwadx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gaoztuksn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gubuuwovu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/ggodlayet.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gtwubcufu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gjtiqoyhv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gtdmlxfgb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/ggodvhumz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gjwnfbpkx.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gbikyayjr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/ggcaertcl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gekfjloor.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gqhevbypt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gzfnoxjna.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gozgfjbwp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gdhzwjbbi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gnxyoflgd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gumtilfnm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gvummblpi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gavxzdvgc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fktsv.cn/Article/details/gkfbsgyjh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/gtgdzyyup.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvuiplgli.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gnnetwhdi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gbahnukxk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gpsilowks.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gkimujyor.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gcqiqlszi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gopmrrtqb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.epnwcf.com/Article/details/gkljzcpas.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gcucynupk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/gxojagjxb.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/gyltiwpyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gqnhjooku.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gxbtgmzuw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gmabekbsu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gpzojuoue.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gslemakkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/givhvbquq.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/ghworhmwk.sHtML


<!-- 参考信息 -->