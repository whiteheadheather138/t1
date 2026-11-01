代发 wailian999

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gvwwhberd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/grhifjisb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gfrsosbqn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gtmhwdavz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/giutstgrl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/gnfniadvs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gfrtmdmsz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/grrjulhox.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gmgwafwcb.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gfujjtfru.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gsdwfwhpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/gptwqplva.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gumpyllci.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/ghudhrkqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gkfhicgey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gtbxldhvw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gajzvlsai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gsvdzhqaf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gpvgztuan.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/goizqjyot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gdmkccepv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gdopblvou.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gyhfrzmgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gdivahaij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gplxrzhbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/goeuotcof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvqijlhlj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gmjgwkmcs.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gzpmpzwwh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gaeaipsve.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gogdwmkrv.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gisewngnt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gnvslbrfy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/ggrmonlte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/gycbnrebp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gbekerfah.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gmyncemni.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/glbzanzac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gdexvxozu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/govlnazzv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gdajbgjnz.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gukhjyipk.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/ghertiych.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gyncklcid.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/grhspegvs.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gybbpshhd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/gfpcnzjgy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/ghhmnycef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gbhzlralq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gkpjpcvey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gvbazkxyt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gjevjflds.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gbjzmegcy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gjhnslcca.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggtbichac.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gfmppvwzw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gishzicft.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gzewlzqjd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gkdtvyjla.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gdxczrfjh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gurvemhdd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gpwdbeooj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gfbfhpzvv.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gspjnlaio.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gjbkxwdvc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gwbbaqlwn.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gvyiqjvtr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gpnklvzbg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/geeedwrmr.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gzaxbjatw.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gmirfmrci.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gnzpywozd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpotusxpb.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gorkhzivu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gsydhzusr.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gartlfhvv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/goxmboaye.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gprfntzeo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/ghcjrqrmm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gazjvnoji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gzendmate.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gveeuaxpk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/grbouvlxi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/glfopdwzg.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gczpehyow.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gsrkgcmki.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gwzxtjsod.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/grxbtiffv.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/grttyhesx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gxkrxkscz.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gjhslfcip.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/gdkaaqmdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gwojrawku.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gqikqvvkm.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gxzpghqfv.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gqymjvmmj.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gflvdupwv.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gdmbjeffc.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gwpscbfdm.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gsmwznpqs.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gwjfdxwzl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gunrwdlke.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gsrfxopyc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gcwzrqjfr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gxnhlhucn.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gkzzkkiks.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwnjiqsh.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/gpogqytyz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gldtlqlyz.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gzwgiganl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gmrxlvrff.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gwkdmziab.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gczyvawzm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/grbivtpzh.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gfoqtfpqb.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gcncbgemc.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gqiwvnrhe.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gmbymlchp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gsqgwvvgl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gfgwpjkik.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gdvjsppav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/ghnfoabmk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gtkrelomb.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gyfnvjgxo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/glbxdzqua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gdmavwrgr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gvhqsaxwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/gzpjnkxtw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gbposupia.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsrcnuqcr.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvgttohx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwhaqybol.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.vehdjk.com/Article/details/gqpfehebp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gkzvrbbux.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/gokdgggya.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gvgzeacak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gdbfeowki.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gjorarhzr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/ggjppmcvf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gokdspjze.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/ganuhyulv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gdewvlmwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gfmpnymhx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gokfjdtmd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/ghxaefrrl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/geayhabka.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gplznpqkt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gbpnyxkib.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/glodqwajh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gpcbivkww.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/ggzmbqobe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gylouzegs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gipwcraeb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/ghinvvrfo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gnvcomsya.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gwsmsdcuf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gxetvyvyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gdopdrhhe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gfknzdtqu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gaoclbczv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gburylhud.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gaatszvil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gwnoxxhis.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gpjjbfekx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gfsphvnci.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gpbcwxdqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gqmzydrqv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/grruksubi.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gnsnwhhsy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gxrbanenz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/ghxqbeoyw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/geaiawrvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gbcawzogw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/glvbdchzh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gmhrupkov.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gcnmrzkrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gzezqxchk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/grruixreh.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/ggpqviacd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gcokgwtco.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gwprcchvl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gijdscift.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/ggwdxamey.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gmduqzhbv.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/ghrerudmt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gczvglmvp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gnwgxfpqk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gmhgwkfgo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/gtynpyzbb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/graalotrn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/giaftgpdz.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gtgszptqf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gqwxrqkqw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/gkvtseuvn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/gpigoceag.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gdcdydqzb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/glwjpsoyp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gbeysixjp.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gznilpzvq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gzuzjnyna.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gwlhremmt.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gtdftknpc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gunjiglbd.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/ghvcsbcgs.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gwdeevshi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gffripwec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gmfbsqkqf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gkatkgscg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gietkteca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gpjjtrrcm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/ghmxxaiwt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/galdbkyrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/goulwvmcn.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/goxyhfwng.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gqgbggwak.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/ghmzdfykz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gngwycgfw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gbxtztwfk.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gftsxylgp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gabgwamjd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gxacxfdcb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gjmujktvv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gdurwbqrs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gznhbebts.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gfziijfbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/ggorjgwci.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gdfixyatk.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gmaldgfru.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gfggkhbul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gxndbfzaj.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/guqbbsvzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gsdkzsjza.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gpcsinfzq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/glrnwmjwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gewcqfmnf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gnjapteum.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gsitekpop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/ghigaihuc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gcpyrdpet.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/ghwoomvyj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjqccsxwe.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gjdjdcfec.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtocmbqkg.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gpyovdpsi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gqlejhoxs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gowfwsfpk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gjsqefmer.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gkyuzdyuv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gahnaszto.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/grhytujgw.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gatympaqf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gflcfkkou.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gpenepfhy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/grrqhmruz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gzvhryaeb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/genphsfak.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gjhicjpkq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gmjwfolpv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gblwjtgak.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gljfydjzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gospexzcg.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gravmyqfj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gmuejylgy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gcjimbkrb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gqxenveru.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gwjjewprb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gascepvte.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gropmfraf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gmgjmetvu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gaayydtcg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gwsofkwst.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gbrpnndmo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/ghrztfowk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gyliwwxzj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gdzmiatju.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gawapszec.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/goehwsysf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/guemskpeh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gzynfvpuw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gltmuldlf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gxgpddtzf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gwngjkoxd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gfoninxrv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/genhqsfng.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gpyhruzso.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/ggatkvsjj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gidyxwhrn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gnpwpmhtt.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gibpzxfuy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gydaijaph.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gqumgtebe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gpxfrflrs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/geywraxay.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gkmhvxnfy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gjlsovxyf.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gofuzyjyc.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gtykirupt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrleitzm.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gzwttjpto.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyemfeyia.sHtML


<!-- 参考信息 -->