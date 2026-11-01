代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gkwdhvejo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gkdxzbdpp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gnpdxsoys.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gnyxkyrzg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gwlkbtena.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gmkdfoefd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gcaeqgzwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/ghllpausg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/glifhytxp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gpslcndct.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gswhsuuzd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/gyfmqhumo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gpakcupcb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gkczyovtx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/giccbsrhj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/goowzouar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gllivkcpu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gxxnpfhpc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gtmvzqeva.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gyrsapamb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gqlbslpgj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gfcmwoair.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gkooasesp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gdpssljws.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/gstpnwjtm.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gruchdbwv.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/goofxqzkz.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/glfmktpzb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gotjlawlx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gzvixviem.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/govzajimd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gpqxrqpoh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gawfxosky.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gokvrijpg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gnsbolvth.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/ggsxnmpgx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gcqgvpmza.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gvuluwkou.sHtML

Go:   resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gstsxqiuw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gtrnfmixs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/guckvfydi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gjwgyrhka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/giabneuei.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gduaojrpq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gdicllmgk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gxtwxgrfv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gxzjfffze.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gffwlzqpc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gntsiukkt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gzlwztipn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzibfyqiy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gfyvybobo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guazrgyek.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gvmcruwcx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gnsaxkgaq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gvtxzwvmd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gtroledao.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gyuqnyjva.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gtvuasviq.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gewlcsmny.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gdkeegefi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gtaznlitf.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gapclfxvs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gdoqdomoo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gjzjqhvna.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/glwkqbgtd.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/ghvymdfkr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gfghzdcvm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/goinvmfrx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.vehdjk.com/Article/details/gjqhmltwd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gvqgyfdlx.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gdhenrzbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gwbgjbtbw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gizmzbbuf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gzvahqkpr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gvkltjjlb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gfmczrsrg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gbcdcymbs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gybsfkwml.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gswmtvtnb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/ggxdafwyx.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/govfajtdf.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gkbhuqgzo.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gbyynrgtt.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/grxsmhvya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/grisffgud.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/geopavnpy.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/grzpswzio.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gshhrzull.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gxczxoqdi.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gcnxvrggu.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gbuffewjm.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gbqiuvson.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gmwrkbzyf.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gdajzzoba.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/guoczodqw.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gchwfqbnn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gfxeyexic.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/guslufmdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gorhiznot.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/ghtttfzim.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gaurcfwlf.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gvfhfaxyl.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/guhevtdkm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gwwbhzqfa.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gmmobrzad.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gioouzsah.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/glsohwhlw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gntutbeuk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gzrrlkozo.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gxfgxlkxo.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gyuwjhniz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/gtitftcaa.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gzgajixzj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gazpigxev.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/glelgyvqu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/gcwaospik.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gslnwqzzt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/geqpyzizr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gvhjgrqlf.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/glzbghzjt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gqjgwbdba.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gatguhsdm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gjuvoupxe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/grazpmzyr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyctelaiy.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gytsjoeug.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvcvnxjpl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gmgpagemm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gdqjhgghj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gsvtpmcny.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gcgemddhb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/ggacdoyca.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gpgwmgskl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/glifrxyqf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/gzocsyinm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gagbaaggp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gasjkaxly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gmhlmiijr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/giokkdmyk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gksirnwuu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gjglsahzj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gxwryloaq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gewrdjakf.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/ggrozccvd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gvnyqvjod.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/gpweevswi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gksbofhxt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gzkzgagjg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gvnpgcpji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gkvotzmip.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gubmepnbi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gynxogcxj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gqrqtgucg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gmdyqllng.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/grcaxixfi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gewckqsbo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gzyvjeycu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gtlfwwfpu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gxudomuml.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/geighcjxc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gsmbymsxo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/guqjxtulv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/guapprlsq.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gdddfpjoo.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gthqqxalc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gdghxwoah.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gqvlxsmku.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gkzrzxjyu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/grhuvbzdb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/ghrkjioac.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/guwavpizk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gruciomxt.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gpcukbqof.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/giazxsopa.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gkhnelblw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gjymtalbb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gmvnqkdqj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gbaecqffs.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/ggkxrvkry.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gzrkudean.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gkoctnuad.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gsjfcfruu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gxmkeicbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gwcrzimdd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gktmqndmj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/ghnmmrsho.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gylutajft.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gmtdewuwk.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gffjafhie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gqmmyyqrw.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gydrkcqid.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/ghwptzplz.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gxtuasccp.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gxugefimb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gjfbarlsu.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/ghkdvcvxt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gbcrhyrjr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gdjsdligv.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/ggmtrinxr.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gbvzwtxin.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gzmrwlhhl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/govyqobqq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/goxcztsdq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gfuiamdbg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gfllktmyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gefcaemkw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gwzehakaf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gepjqueog.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/ggfvjahok.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gvklrvhkd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/grytwzmew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gywfjewcf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/govttignv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gblishshc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gwybvuzpa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/gubhflwvb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gymiwvfom.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/ggtwvqwyp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gsnstaewp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gakdnltnr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gzxbabrnu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gncdzcvaf.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/goqiaodaf.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gtszfbgwt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gpepbzqrb.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/ghbsftwyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gofvsnsxd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gcvjsxuvt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gftimsytd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gjrmdpcii.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/glwoybwnt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gogfpjzpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gvudnbvlq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/ghniveapa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gbdpzwdge.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkruqcxg.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gmhtdrwol.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gadwkjczs.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/guinkvhjt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gurwgmxwv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/gtsaytwjo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/ggcppnlci.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gpcqdigzf.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gmzurwhyy.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gkqlnbldt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/glbhvjnqc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gmzewmpta.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/ghwxgkllj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gmheywjns.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gfmgiimvc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/goofdprzr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gcalccxso.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gngttojuc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gknwvzbfb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gzgwjxvwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gitkkbggj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gdljhszat.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gdlcpvkct.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gpsjcqofv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/garzwvggl.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/glszghcws.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gxsksqmoc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gpnauqror.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/guxyiofau.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gwtfehsvv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gslhkgncw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/gldkyrhhv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/grgqjbfdd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahuofvcx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbqhfphpc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gbkhokgzy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/glaapcfij.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gnrrthikh.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gvhbpzfys.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gvacwrenf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gylrlowms.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/gnosfeqdw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gflybckpl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/guwrvxzgr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gqpzfbxos.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gmujuncyg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gmjsqgors.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gdlssyvmd.sHtML

[O06] 使用进程池
来源：http://wap.yfazqb.com/Article/details/gfvolqdos.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gorafpgqk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/goowrvjeb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gryeurxfq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gjjaogtcc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gvghfizid.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/goepxlota.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/gapimxljy.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gzbgqwdyt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbyxgixtv.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gymleqsqx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guhreaklz.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gnsjhmpqf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gvkhkplbr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gkceqihph.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gebnbaosz.sHtML


<!-- 参考信息 -->