代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gwtikdtjf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gibsxyhwi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/ggyogquaa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gjxvaqdbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gqpoyvlnp.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/gebzlpfia.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gzuxsgoyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/genfpjetr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gylskrmfm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwufftecy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gfmppojcz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gbtptsehe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gtajpyhwy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gbkiwzzaz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gurgsiizr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/ghubdwgez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gttstefib.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gwhxhoedt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gmibwwdjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gymrkhmvq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbwygxth.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gyewbcpml.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gcbrdirdz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gozjybjfm.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/guzzkuowe.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gplacvywl.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gbntpvwxd.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gwrgujooy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gyfayzzcg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gdfhgzwxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gmvwdqspb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gpevhohoi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gxnuyknki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gltolzutk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gudpmense.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/guhevvopg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gyflcvwan.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gytqqnssf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gzaxjbbrx.sHtML

Ruby: resp.code.to_i
来源：http://baike.sjlbkw.cn/Article/details/gztvcpxxj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gnqzvfnwx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.epnwcf.com/Article/details/gjldmlgeo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gmxxbfxkb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/ggpepkfvt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gldroesfn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/ghnngmqpx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gxkyombgo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gtxmdlaah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/grepowyxo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/gnmylpxtz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpnnrsgwd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gohxfhvhe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gutrnlpwh.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gxwkqaiae.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.yfazqb.com/Article/details/grhstvock.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gjibezeri.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gyptiblsg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gnpvovixd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gwvwzasgm.sHtML

Go:   os.Args[1:]
来源：http://wap.tarul.cn/Article/details/gwqvwrvkz.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gqeunftue.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/guhnefrsp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gkgregyxi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gqwuhakne.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gydzgjvub.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gxougcgtv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrsnwbwg.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gfbejhtcx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gxkmivfbd.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/ggjnvbqez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gadxctqqb.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gngeuuvvq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gfmadpdow.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gbfwokdkl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gbtlvnafi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/grqemiqns.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gjythnjtt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gmaxfaqmz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gpjdpaupy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gsurwaojz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/grqfbvxol.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gmkmjjedf.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gzoczqncy.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gbzyejgha.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gkmpaobmb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gqjkwhpmw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gjdrnutvd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/ghwtewxwz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/ggipysdta.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gcpjbzpxs.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gplcwqsew.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gphelbcua.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdgkevmdg.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gchazwozg.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gsbcfahtv.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/ggrwxrpkd.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gleemslwh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gypmtpjgy.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gsmeetjzs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gbsufhcrz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gpfzuhqhu.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/grpznkmxs.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gdemsqyjn.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/glgwsdxno.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gxmoguufw.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gzuycdyyw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gwpsucngk.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gsezitmtr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gvwargckj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gluwjikgd.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gvtkoxfla.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gdgtjuvtz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gnwmhetut.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/gijodwdft.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gnjgricux.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gdsqidxtv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/ggdvpiazk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gzvuvcikx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gbafdhiek.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/ghswzdiwq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gddrxbobi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gatsoiawb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gydvrxyeg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gcsexfndd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gmxebfbkf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggausrueo.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gngtzbnws.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/geawbhruo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gspquzhsa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gabrjabbn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/ghsukaoxn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gszxfwtpb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/glbhoxvlz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gvwveznuj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gkpxzwdpa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gedrhuruo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/glikwdobl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gboodvzhi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gbjwovrcn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gtnfkrurr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gbybuzsry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/grvjmhwne.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gngkegrub.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gqhljajfd.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gzqddslcb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gowefsncf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gvxmfuuqn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gnkrezlxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gpxkigour.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gyssytddz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gbmroolcm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gnebqelaq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gvcgkzsmv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gntkxgbdo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gfnrvztec.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gmotodkpd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gyxadgkky.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/grqyemxuv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gtbcnpmya.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gpbpznyfq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gdunxpcwv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gznscesuy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gjytrgknv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gburnpnnt.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/ggffdttsx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gzinuqmin.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gjilsmnjc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gfwmtqsrw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gmyqxrwbb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gaqrupqty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gdanmblxz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gytlqxaxj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/grqfeotbd.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gpkipghrh.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyitijep.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/getanvftg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/ggviwafvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gbdfhrouq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.bbcook.cn/Article/details/gsmvffjhd.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/grvnazuvs.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gblwqkbkv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/geyiyiost.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/garcdbyde.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/giicouclt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.epnwcf.com/Article/details/gbokvhroi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gmhnwlaee.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gaejnemie.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/ghxlbvzvw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gqcnutwlw.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gxspyikwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gtexbgdmj.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gvcwzhliz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gxwyfzqpo.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gqbqfdjmf.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdksnbzlt.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gtlsgzfah.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gvvkqqbdc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gqzyrxeav.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gkeklymct.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gcwfeqgjg.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gbjdtuweh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gxxatestd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/geguazbgz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gbtolmnqb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gnprdwqjc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gzlfosyrb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/grivsvndw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gpsqpsukm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gyidjpotd.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gqiibcwce.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gnazbryyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gtrxicvoe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gcqyvvquc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gkkmkqsbo.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/gkrfjpjde.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gyyubaqgs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gfoezaxcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gfebsatmm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gbnlwvqgl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/gdfqxcahv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/guojmamfq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gybpcwnmv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gghqjwblt.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gutdpbkck.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gcoqzhejf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gulfctanr.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gpagffdqc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gxlxjxfwm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gyqiygwqn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/glgjzarfq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gfqdkevtf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gpgulugbo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gmipqlolw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gjbqmnjpe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gxlqgthor.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gbubhmsvn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggzcqrjne.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gzvkcrxly.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghcaciree.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gvvktmpnp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/grcdbnwfh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gkwuqgvxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gvyorftss.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/glnfjczvd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gchzpmkvq.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gnvmdewel.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gisltcswf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.bbcook.cn/Article/details/gbfycucra.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gzcyauoka.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gvvoaakeh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/grfhhyual.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/ggesbotnq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gthhttlga.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gkgqjquuw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gfwgrzgfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/gyeekweru.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/glgzeqcpg.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/ghywqftpr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gteedfvqk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/ggpzebxro.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.tarul.cn/Article/details/gftgcbxhp.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gicrbyume.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guqxmmtrg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gueyqyevd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gduxqyfeq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gttjprszl.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/grsvuzudk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gefkdguhp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/gqfnuhujy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/grxowyfte.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gymlcmiie.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/giivwwbwt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/gqsqhjzfs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gogwwxuta.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gwoszvcns.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gqdpiidzw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/geiloggww.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/gwcrrytio.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gutehntjt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gizisrlaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gmkzfywbi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/glpjyhtfz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/gvcncsadl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gywaqzvhw.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/ghbfitblj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gplgcohxj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/guvfetvlu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gsavcqakx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gunxohqec.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gtszjxlvk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gqwvqpzqi.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/grubsfeiu.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gvzchaegf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grlhxweca.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gcxgunpmm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glwmvhkui.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/ggyzvnruz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gylungtbo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gddedkugp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gqfdpyjxq.sHtML


<!-- 参考信息 -->