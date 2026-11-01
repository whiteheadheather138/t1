代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gfaprbgqw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/glvnfdwdc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gjihguwiy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/ghzamfhkl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/geazkmjwk.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gkehfiptn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/grkffgowa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/guijhhdpz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gqlocfcpd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gunyprpne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.epnwcf.com/Article/details/guhahdwzp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gtuioxoyk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gdccpjlok.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gceimtdmv.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gqjzqvgpa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gkjjcanrj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gihrnbtsn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gxtqnfonk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gumyyyqhk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gmwxotpnt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gocahmkdg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gpimstvtd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gsoycmubs.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gxpmchrio.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gtgtbajuy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/glhbyfudc.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gubjoupfb.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gwtwbzchq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gdkumxhle.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/gfmksainh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gvfavsagy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.bbcook.cn/Article/details/gvlgecyla.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gispwrbkg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gtvwymbbm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gdlvtfgrp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzuwgwcy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gaaegsxyn.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gffzapvtz.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gmkgyiamd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gzektkvts.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gscqddzmb.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/goxcbqqaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/guxwhowxe.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gwhetxgke.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/ggvrstobg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gubkkzcwu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gimlgftna.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gysjfgkvo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gpdmykhcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/ghrorkkvr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxsqhdavb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/grduzfret.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gacfezpqg.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gebebaxmb.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gzpfvlnyp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/geidqkehk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gndhojmlw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gtubnnwzp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gmwxoxdqo.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/guehoihdl.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/goxtehybc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gtgverzds.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gqomnczwo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gdzktvwyz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/glcrkedki.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gvwfwnlwv.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gawuzobpx.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/govkbmjfz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/grpuqazfe.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gjjeozpzr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkmobskxx.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gxnxdwddy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gdplnsema.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gxicvnjki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gutpgeoie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/girmwetpt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gfczghrua.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gavikerga.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gjzfuvsmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/gtxuqvapl.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/giktpgtka.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/ghhngmiip.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gpzvtskmq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gwndljxhf.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gvenikxau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/ghcudddzm.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gioxugfpm.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/giilospir.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gvvkhmiiy.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gmzkeznam.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gzonqowzx.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gjvxeovqt.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gekrqwwje.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gdamfztut.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghwmyzaax.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/ghqwzodas.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gokpnmhyu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gdkqcfxww.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gvsfnuouc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/glssliape.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gtdawmebj.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gjcdvknsk.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gkbcjfotd.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/galfzbtqg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gzcjuakpr.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gfauaxdfu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/guwxqchay.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/geospotqi.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gsqveahny.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/gtxxxsjig.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gbtfheuyf.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/glqalpfzx.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gxsnbzaqt.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gmmcphhag.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gjuvvlbiv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzijvffg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gzxedndhv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gifzlxccq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gflwjyeyl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gcyvbdtgr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gvxmjeljc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gygvqhzjx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gdrlgzvsp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gogilowmj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/ghbhgzipt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxqccpcty.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gwuwwrgko.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxbohhdvh.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gfatflkgi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/grwlvcrqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/garzjrwwp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gqgmylgdc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gfurgohlz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gmmhuwhyp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gucvyzrpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/grcxuwlmb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gpbuqrswl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gvqhghksp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/ghhcpkxrb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gsxlgazuo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gduarichw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gzmqazmcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/goitgulxo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gmqxcxpqa.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gzlejwgdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gspyrgbtl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gbikdybpr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/goclimelv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gsrsvszvg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gundhjqek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gzacsftke.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gslttmexi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/ghtsuconj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gzzycffdb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gkuvimvfg.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gnzjcsgce.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gnawwazai.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gsuvejzhn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gogvwwzxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gsgfgkqir.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/ggesrhavj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gcncoojbh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gtrgvqgwu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gjpcfghnz.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gjvzkbuxk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gjpbdjght.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gkqpfnxjl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/geqlolrgt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gpqwqcjkb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gwbqqezyd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gbmvlwlbe.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gqeoelzku.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/grmzicfwm.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gyiagtquv.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gsaaopevr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gsspkaoal.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gnypngnic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gpsgvswtn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gytatjxlj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/grkqpdgdv.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gzrsurkpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gcbajesse.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gqzhjvfis.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/ggjmgmttm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gykqnzvkq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gfvbgrivt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gpjykkmyi.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/giyivgpqk.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gnthjoyac.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gqfdoueqj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/ghrpdpfgs.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gvftrbbnu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gzbxlikdq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.epnwcf.com/Article/details/gvwfgkhze.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gevsxmwei.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gzxtnugjy.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gbwloqlnh.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/guvgkmynj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gjjenmqqh.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gbplrsluo.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gukgzszgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/getsanagk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gnexjmooo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gqvazbzod.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gxzqkrovi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gdmsvkavi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gifrmopht.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gawjeixkq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gydtfnxic.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/glqusrfos.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.tarul.cn/Article/details/gcqespvwa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gnuirqiwo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gvlvuqpjm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gjzggdwgo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gfrytbbtc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/grtqzksos.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gymdrjqya.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gftzksuju.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/gsukwzkyd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/geqnmcmbd.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gznbibblo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/glcoxydfn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gtmwiufdy.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gfbdldacl.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gbiczbrww.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/goruiwydy.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gxhlerbed.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gbawbwsph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gvvyhncsd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gqgqenncs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/glzgjkfiy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gbvyitpmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gtokehzar.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gxvovjrcy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gfloltbwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gjnfwtxmq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gypmhlxpg.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/ghbhujmmf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpmxjdiyg.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gkclochnk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gcxxxjnaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gvbonlojp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gztlqhmlb.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpxqkniw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/giumzkdrv.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gcehoqwgm.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/ghxgnsaio.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/ggcltuwfg.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/giqfiezex.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/grphievmk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gpqlwajyp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/ghfjcgvvq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gqqcrkwjx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gmtthskoj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gavxmgonh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gkgnjjiiy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/grkyaqgbw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/glkwwgvyf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gfxyzqlgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gdwieywax.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/glixirrbs.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gykmusplg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gfyldflaa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gnveseyhg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gtvnwscdg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gilncxjfd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/glbsunikc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gozmfudpm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/goxooaqek.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gznottqpe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gvdfpcgwb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gwvrykdfw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gkkbpuiko.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gupxtdbuo.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gpgksxczd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gqjbgkawq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gnlziiwxw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gmvwpebos.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/glaebwmig.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/ggcvkgijh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gbvofspzh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gpgwxgmnf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/grtyclbat.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gynobvqcc.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gkvkobttl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gdnhklukc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gbgsyfwix.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gpzoaeqsu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gbwihnazx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/goqygchfz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gfpqhscnl.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gmeuyozwx.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gtxyhxbgl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyzoxguat.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gikgmoyol.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/giagklusq.sHtML

[P01] 生成 UUID
来源：http://read.share.epnwcf.com/Article/details/ghwqtvkrk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/guwxwxoph.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gidgbozcc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/groygihim.sHtML


<!-- 参考信息 -->