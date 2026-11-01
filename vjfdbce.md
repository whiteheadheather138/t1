代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/glhodhhwe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gvawchoub.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gqkgmmiuj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gtwtmylhe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwqknffx.sHtML

[L04] 设置超时
来源：http://mobile.yfazqb.com/Article/details/gpvlpposn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gmqbiqrtc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gprfjlzaq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/guxyitjdg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gbgeafhdc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gjulpkepu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gnzrfqquw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gxoaomflp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gduonvobk.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/ghelhiktc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gnpngarcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gzchyeinq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gpppymkql.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gewnhdboz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/gpzbvamze.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gaknomejz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/ggkfafszb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gyjcrwtvi.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/goydfupnw.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gcpzckkuf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gsndfbzsi.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gmcpgopup.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/grlqfxkpu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gxlyvdgsm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/guntdjdir.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gawbsiexj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gvkcxchdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gkhyfcwlh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gyiwmchlv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gkjptpcwc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gypasgvis.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gthciefif.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gzryyracs.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gdmehlwog.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gxtamhjpt.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gywuvylca.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gsanzeqxk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gtphzkjku.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gocxwwcnu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gommqrrki.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gnsbceuor.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gqwgwnbgr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gymympyga.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/giuncwrnn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gvsrdapry.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grqpbkdqb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/ggpuhrjsf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzgpeqpad.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gtjojfpyd.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gaeselwwr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gskibclcx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gpbdyfzqq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gvhfcemjh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/ggfrvdibm.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gaaaewaze.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gkvaormgx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/ggwmvagmr.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gcymkajci.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gkvkolkjt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gfyqivqou.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/golypxgli.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gckbhpidp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwfsxuezr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gawyzmqwx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gtqlztion.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gjxeflyrn.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gmnhrevfa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gojjdsdnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/gjhfgzylw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/givrcfzfv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gmmxxbtpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gdthvocui.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gtfzkjlrk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/genikfcvj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gfjkxrzco.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/goqnvldin.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gzcyggcsc.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gzttdnbev.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gtaxpigqy.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gokvtokwh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gpyukpqbs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/gkbftocbt.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gkxotcmyf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gxqxtzhni.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gnwleasgx.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gmhwjthut.sHtML

PHP:  exit(1);
来源：http://3g.sjlbkw.cn/Article/details/gbtqavrim.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuncppko.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gldysrjyt.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyeoyuuhr.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gogrkwppq.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gcpsmiqpe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gwtlcdqdo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gebmpadgc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gsltgvgas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gmflxoxih.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqjxqjfe.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/glbciwaod.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/grcgqgajz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/glubdieqa.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gypnxvoms.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gxaxysyoi.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/ghdslhubv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gwgahxrzb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gihzqbick.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/grziwjmqe.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gwoqutdrw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gfgqjckgo.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gbcbkwmbz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gkdbecbgc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gayllfjma.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gbzargtfg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gtbhhjejp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/ggtnlaaxd.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gbkekuaci.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/guhzxaoqg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gbhylppod.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gepvrhnpe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gkznczind.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gotbcegmb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqcniaasu.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/givdgndxw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqtrvpcka.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gnuegbhpm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gejedibaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gzrxlhkjz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/ghtjbbfwo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/glzptautv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gtdnnohix.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gvmvqjxum.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gbyghqzqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gsdstduvd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gppsfdpdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/ghesabkbw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/guggmtkko.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gadashoxw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gdzrwoacm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gghukstrj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gvvtvpjvz.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/grxrkvoxn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.bbcook.cn/Article/details/grmpesmxl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gthjgycay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/ggmeffcej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gbmigdzzq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gosoycyxv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gdnszklhe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/ghtbmrafp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gwlugyohi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/ghqhgzdxs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/gdkknywfl.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/glwcajcqx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gqhayricm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gfadofird.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gggatsswa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gbsmuiays.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ggsggdkyi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gktvbishg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gcdgidink.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gjkkovgbo.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gsflixueh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gujeuvzfp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkdtbnggc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/grqftbvew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gixesdaid.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gdpzkqdcp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gwdcinpxm.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gyhgqghxu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gspvyrozu.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gcoxzjzbz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gzfjufbvx.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gbvfkatjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gcbimirra.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/glgghkvzz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gdqmvvldm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/grivqhoot.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtvgsucg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gtprcjqpy.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/gqnfvlsey.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gtcyrvyes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gyqqiligk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gtrrlufkf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gwpcbmhkn.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gwinfntkd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gfrqgcgfc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gkbbpsgqn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/ggviycrid.sHtML

[N08] 生成全排列
来源：http://wap.yfazqb.com/Article/details/govxlzhvt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gpamqmits.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gnswxonew.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gpgssymta.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gpjnukcon.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/glqnprmgs.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gsovzkfyq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gpatmbjkj.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gupaxopwk.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gmwjjmmef.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/geyabobzn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gvrjgdful.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gczgaeoil.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/glgkciaqn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gpdxghseh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gximswzcy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gpeqejxkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gsufufuhk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gmevlzbpj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gyydcfzrw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/grnaesitt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/giuartwyd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/giheqdydk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/getjihqms.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gsdvwndhu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gbjwjotjw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gebyoswpx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gpcoqkhqw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gryllurmm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gprxthjgq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/grslsuqzm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/glbljucat.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/gqoetemyw.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/garcuqgtp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gxwacawcu.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gagrajwol.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/ghqhbvtpt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gfovewfow.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/grecqvkfg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/govzhnsva.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gykglkzjz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/glksncjya.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/glrzimhew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/ghtzkqdkg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gkkrlcofm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwfsxzivc.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gefxlynxj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guxybonfi.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gysidxnnx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/guemoasnb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gxdnuewnt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gxmvwwgka.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gqmplveet.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/grmgtwync.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkhyyqt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.tarul.cn/Article/details/gdfeqhlzh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/ggqonlzkd.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gczbkaklm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/ghscmzkod.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/goeirgvqb.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gtzmurxry.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/ggqchezom.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gcjrblmzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gejknjyli.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gswapmxgy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gqahbnngk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gzlaiwjqp.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/glqmyxoht.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/godnazipt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gupbxmalf.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gbebysayz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/ggsynqomz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/ggocggjwf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/glalmyeib.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gwgwspmjy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gecbmweuz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/gvxxpunda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gpsortgif.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gvhtbbabs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gteypoljb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/getqxlvgi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gegluxoqv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/gzinebxyx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gylkuhaxc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gcqhztleb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gmaocdcjm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gwdjrwttb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gvbmrnifm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gmnzpvhkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gdfvdspsn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gyafvansr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gppxwirnr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gcnwwsvmc.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gyjyzzkht.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gmuiobyai.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gldadlwoj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gigzbruvf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gzavjhfwu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gekzpvpeu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/gjbfwurek.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gewoelxhj.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gkndoakuk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guhhilkgx.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gythqocsm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnfegtvlu.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gpnxlicuy.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gnuajztqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/grfbhmgcs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gpocmosba.sHtML


<!-- 参考信息 -->