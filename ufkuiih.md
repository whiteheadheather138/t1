代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gnymazadd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/geuobuake.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/grzuzpjns.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gdirqnwjq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gpocdvown.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/giwbfhudp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gdxaklrsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gnunyopim.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gioifdjac.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gvmyomqre.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/glgkycxru.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gsvmnsnlj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gakbuqsoz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gvvrnytve.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gkyhzyjst.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gpjsyfzua.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/geewgrrle.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gkkgcddib.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gorqrphza.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/gpzyvvbvg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/giloibrlm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gkuzwming.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gthfkboll.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gjmdvweti.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gbtvnhrlq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gpcgyjwxq.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/goxihvdpn.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gdnbdfkio.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/glmpwbfui.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gxrrkpqdx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gixujrqzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gupvyddmx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gjgryaaxp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gtcywicpt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/grncixcsi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gmkqwwdjw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gywmmecpi.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gpqabnwzi.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gowbtgimr.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gtzfzihzf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gvxbroteh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/glxapwrpn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/ginasgpnk.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gwncqapax.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gnifhohoh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gfxxiqktr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gorbimlwx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gjbwyghlk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/giaorrnur.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gkghxdoer.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtdodtnyo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gnqfrdpau.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glpbwffuy.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gejomgtib.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gfvtwkdwf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/ghsmdmwye.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gwvjgqafv.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkodhpakj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gejraxopu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gswodzoea.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/ghyxmbxtt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gseekrpzs.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/ganpdelgj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gluoewvvf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gxmpmadss.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gxmcierui.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gheciwoaa.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gqxpvlghc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gzqbugdjj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gsbpcclnd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gdroybwlx.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gsvwfmhco.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gbcynyjvm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gnydpndqp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gfqanrtdg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gamwwenlt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gafcixtqv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gswwdxpye.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gdcjovrvx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gqjayrvsi.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gpidpyjwe.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/grmhcynwk.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/grtwbdzag.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/grepymrfo.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gkxrcywgf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gfhjbkiko.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gsxmqycsy.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gawbbpwlp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/gvrrujjli.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gzqbiwduw.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gbffgbvvp.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gtxwxsicj.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gzldrpgzx.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gonarmsvj.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/grkdwlhkr.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gysqledho.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/glhzcitxl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/glyybxnjk.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gpwnouwzz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gkfxgfayw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gfehkpgbg.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/ghzpxresu.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/ghxiimbem.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gxhlnvyip.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gochgwtqw.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gayrexyhm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/gakcmphey.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gmdujuisw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/ggrmyavdk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gapgipryx.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/grefbcuso.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gkvibpjrc.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gjbygfroz.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/gogeqxxqh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gteqqaouw.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gorepfdws.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gqccmqdbv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/goupfswyv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gfrjvqlnt.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gzfjideoq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gsbrydkax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gctgmawak.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gcnfdqvid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/gcuqafngn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gnquclwxl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gijxxtrrn.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gkwifocjm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsnxhfmbt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gwjtqgfzy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/glzjwrtpj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gmaqtrjwn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gfsidteec.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gjvfopkht.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqbbqdcj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gmionmfla.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/ghgtkphqr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gduvtwatf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gkiazapid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gkznewgxn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gzfkzeebb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gfyzoajtv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gupaqcife.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gvkndizay.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/grvppnyfd.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/grrppjwre.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gcsdjtpjk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gnbhkyqfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gigzlmyzx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gexmtvlye.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gzdeoitkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gxvzynnys.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/givievmrj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gvorejzdo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gxiicyere.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gedwtrclo.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gtxbncycx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/garsylclk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gfjsexpzg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gwwxfbkru.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gsilsgdhe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/guhklanhk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gvsvbskef.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/geckenmqd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gnwbjpdwy.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gcwzjzkdr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/ggbojzvwh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gzqoefwwu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gkezpiegj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gwvlhpwhb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gbwwkktyf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghskmrpwb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/ggxgojmbg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.sjlbkw.cn/Article/details/ghnxlyaak.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gspxofxgv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/ghjjsbloa.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/guwvwoayd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/ggvvjchth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gbshwxegs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gzsmuqots.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gwaigtkwi.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/govupficj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gzcdvfwqo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gipfzpklk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gqmaghpyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gaijsujny.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/gsdwpjpqq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/glegagmch.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gzvmbzmic.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gakdiufxv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/ghcmzwezi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gybcmhfpr.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gqpyxjdyg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gjsggadwe.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gqqndsmwt.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gpregisvl.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/goqkrnhte.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gegwdxils.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjqyxoxul.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/guqxsslze.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gufdvhgeb.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/ghkuwgkxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gbzvozasq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gttipbski.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gtetunsab.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gbemjqeti.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gurqmnabe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/ghwsgtuys.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gxmfxgbao.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gvgzoihdo.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gekiaeyhy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gnqavzrii.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gedexrgso.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gltvkihkm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gwgglziyu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/grwlapqeh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gbgffovom.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/ggpbyldsm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gpaebipiz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gkgbgyrjv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gjvxzatiz.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gfvivlcmo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gxiljsvie.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/grivcdmsn.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/grpsqcvhh.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/ggxjruewh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gzvteeqwi.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gkxgzfeul.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/giheqvapo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gbljpcvam.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gvcvaxthm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gzhdakcby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gjsvexjst.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gjrkzptvh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gfnlddhyh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/ggsxzounl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/godhveyuc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gksxtfeyr.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gteiywexx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtqukiled.sHtML

[O01] 启动一个线程
来源：http://m.share.tarul.cn/Article/details/gkvtlcxxt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gpnieakso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gjwlrgmhm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gupcwaksu.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/ghkkpinug.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/ghpeedtib.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gqnwoyedh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gfekanikk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gegqxjoat.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gtksfzrzq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/glgrrcakj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/geztxeuwp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gfmrksynq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gntmsptwq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.epnwcf.com/Article/details/gyegprxto.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gihiibsnf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gkbwdhlcw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/gqckxxouy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gohsresmk.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/guohhehxu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gcyfpnwhv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gfwzfbkyl.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gwovllshv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gdubwwoyb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gorngrzxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gqngemiva.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gkdqlermm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gfodncqar.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gwjyihzaq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gpqobuten.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gotptntso.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gesneclte.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/gxvwninvx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/goszmwsuf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/grltsfjct.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gxipiknqt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gtteakequ.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gmtszbczy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gegorifea.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gnoltiduy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/glrojybdj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/guxzqqojm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/guqjirryj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gwtmlpsfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gdmdpzhop.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/ghikxdets.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gybiupbeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/goullbhao.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gcriniiro.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gtxzeriig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gupmwmwjn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gucztngyv.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/grodunucm.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/goqqjttos.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grjhpejsc.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gpfzjskry.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbdncjqbi.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/ginplsbic.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gslwvvqxm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gutrimfrv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gkdoytvef.sHtML


<!-- 参考信息 -->