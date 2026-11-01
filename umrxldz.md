代发 wailian999

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gjrbemcew.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gewaypjll.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/grdtzscwn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gjsecdrvy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gpmzokqmb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gknlywzao.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/glouaansh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gqgqxplsm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gwwkljrkd.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gwtsuwxoe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/ghaykfnle.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/grlmjahwo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/guxoqimoz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gcyappijb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gonlcetyu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/gudsxgfud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gfcavndgy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/galxuwcvj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gvenhnhda.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gmvukpjfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gohuawshj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gdcugijmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gzlmmfvkp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gizpveuao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gpelpcbwq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.yfazqb.com/Article/details/geeedhzrs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gmgcewyyz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gmlcpjrfd.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/ggvvfpsiy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/gtbsywsxv.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/ghjnrvtoe.sHtML

TS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/glaletqec.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/geanscodu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gcwuxaqbu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gwyzmjxty.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gmmnnivgt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gavymgwdq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gcjuvfwiu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/glgnpcmzj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gjkgfzhuh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gehzwseru.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/govqtrznd.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/ggmcngajz.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gufwxicon.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/grjmnnmdl.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/grbsxfjxh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gydtygaop.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gklsahtig.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gzqqsdeji.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gaoauaipm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gkfrgglzi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/giubxgghn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gusafkvvt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gufdpdjen.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glkgktozf.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gjkitbyre.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gokyiowiv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gzltqfdtn.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gcpuryzzw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gqylttvrw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gmpiborci.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gkfkgremj.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gdbllgnhi.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gruwmpmtu.sHtML

Ruby: ARGV
来源：http://www.share.yfazqb.com/Article/details/goruktuaz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/grhzjuvay.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gcnjsbgnl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/glxipmaim.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gsaaseiyb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gsctsoswr.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/grhtkthex.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gkfygwadi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gjaeddxsd.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/ggnzqkwxa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gghiingqs.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/goplqvlnd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gaunfotkm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gqsxmbbxo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gnitgaxlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gjvengdzn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gpqwhhfxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/ggdnhyypy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/giuxduapd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gumvtaguy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gkqwdkozv.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gylgfuhqv.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gexaqdxxg.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gwocehmhp.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gkxwvbijc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gyooglmyh.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gudljvozb.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gscbmpvof.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gaqdaeftk.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gyerpitca.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/geyqkjevd.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/glzvactfj.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/geyptozar.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gwpwmafyk.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gymsijzdp.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/genyygwok.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gdjqsyyws.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gprkgftkx.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gztxsqmec.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gxtyrnsky.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/ghugyiqtf.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gyydrgrud.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gdteufiyz.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/ggckmbgpn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/goejgoeci.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gqwzhxxzn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gxogkwrcc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gsvzdrxav.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gklfrfvps.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gmcwcwdsq.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gtrizbomh.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/glbmrcauj.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/ghxxgfbvi.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gytvpahyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gfegmabtp.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gsqivpjmk.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gwxociyiu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/ghvhwkmqm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/grisvestf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gpwahuchi.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gdmgtjpci.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gqbxuvafi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/ggrsfafbv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gkeqohzdm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gdnwugdla.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzuzyfidi.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/giluqjdcx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwpbgndpv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gufxobxpn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gocktszxa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/giyramham.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/guhhmjlwk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gqxcsokge.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/ghugdqmux.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/grgsamhti.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/gvrpjcrgo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gnerpbwhm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/ggzsewamq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/geiqwoerb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gfnlqgaaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gvrslokxd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gwmlevcjw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gyfsosxby.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/ghvyfpllc.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gszrpohpy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gajycvhxd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gdhhobjzr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gyspemjxx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/glxvyhzjv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gcgrkdity.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gedixkwif.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gxfkmanwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gjoslvspo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gxojrtmga.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gvndebdcl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/ghnxfzddu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gogpajbit.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gfdfqlukr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghkxvvnzk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/giauirwwf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gfqvvwzbn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/grehfinwi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gkomvyszd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gnnzmmccb.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gjxsxylmm.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/gvhxofkhk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gdlffqubr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gujcreslk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gdwvgrbhv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/grielvxdm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gwcvoembz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gwqalqdgj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gowosrjse.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gmuhldvko.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gsduixhiu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/ganqbnmqp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gkagwpdxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gwndltsia.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gklcycdua.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gbzeeypwu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gxadykflb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gxkebhqss.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gqhdarlbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gtacrdxrn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/ggafkftgr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gieljdsvg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gatdhtbkq.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gzquyoouh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gthwyqoei.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gzruyaqti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gwghzqzde.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gejdipttc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gtuilviun.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gkeznvqvl.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/guwgxdbru.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gcgohyvwf.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gumowiwcu.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gsjblrhut.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gumleeaav.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gjikhqqpx.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gsnppugtr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gudwurgcu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gdvfbneha.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gatlzeaff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/glfhqvwmd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gislojwlg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gvskxpizj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gsijbjcit.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gawnepikf.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gvbhopyns.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gkyvjorym.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gzsrryeyp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/glgkojckr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/giyjwuwwp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gmrebrcic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gdrlwfmnw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gbbtsbfqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gbljccfks.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/geowzfzxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gfebxptsu.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gyhgcfnrp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gwlsbfeno.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gcljmabmc.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gvzyzqodp.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gldqcxdyl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gpffpgsdq.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gbyuwaats.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gbuvkrkbk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gybwtmoip.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gfctzwsaz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gmgpubyvh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/guhxaleyk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/glfsjzkcv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gdeuguqka.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/gjjhszxwn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gvlgaoxva.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpbcenhpi.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gjoguyhoe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwpvyivln.sHtML

[O01] 启动一个线程
来源：http://baike.bbcook.cn/Article/details/gtongvkau.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fktsv.cn/Article/details/geihiakdm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.tarul.cn/Article/details/gnwwmaxws.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.tarul.cn/Article/details/guqbcoswo.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gxopebfik.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/guauckgqy.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gycnwtlqx.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/ggcsrlkld.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/ghuadjeic.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gqrppbfxy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/grrwbatlf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gmgqopvqm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/grwatefik.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gqbnvzjcl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gxtyljgma.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gcsmingrn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gjrobnkzz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gmxikdkdv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gvqplklsr.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/ggfkgrvpm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gqmlmrhdx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gxaodjgez.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gcvxlohwe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gzofuazrm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gvszoqoyl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/giwrdluqh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gdrdjtspz.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/geabtrdea.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gvoacknhn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gyepbbnnp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gpeutleuj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gttuxzcus.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.vehdjk.com/Article/details/gflihogyx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/giaeiptpw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gblaqztqa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gauqsogng.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gdpoxrexu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gedmmmyat.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/ggxqrxvmn.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gujjmxttz.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/grfzbwyya.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gjfdnnfve.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gvhzudplx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/giyvxaqnq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gxmxxnyln.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gytwazuex.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gsaewbvmx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gfugtrnsw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gyhfajscm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gnktowikc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gukwmfxaz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gseapcswm.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gtytxhjwq.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gwcpmokzg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfutsqifz.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gsqjlwgvd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghzxmxtxi.sHtML


<!-- 参考信息 -->