代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gsvdzgpos.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/goxamlwgz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/ggipnpsti.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gqncftwvf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gdbtrdbxp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/grougiwqr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gaordjzim.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/gpjghotsw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/geccnhskq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/ggockppxs.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gwejuqpzs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/giqdumwhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gmjarmtaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gdxsubakr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gmkpgoiii.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gvueodpnq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/gkrbixznn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gnvogqttf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkdslluqq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/ghsxiavrr.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gaovpqdct.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gqidjxfmj.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gpscuvoez.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gkccdmjth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gxpnjohde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gicplztoq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/grixmmgjg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/giebhazsy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gkjkluhwp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/ghsvliemt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gnfqvrtgq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gwomsepqg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gckhryaid.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/goteixnym.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gvkvhvazm.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gchmbhhru.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gspnsoyku.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gfbknsqqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gpvhoedtj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/glnccktsi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gvtxagydl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/ggxoxyqiq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gowqiosxm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/ggnofpomn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/ghdtjmyfj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/getqzabtk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpafsxefr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/guhjpcjgw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghjdxwdud.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gdczszexv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gcbhgvqaq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gpylzwzky.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/guoeyhahm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gkwgllffb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/guwovnted.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gpoopauen.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gkhxkgpfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gjelheuiq.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/ggeoncuzw.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/guvovajep.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gjaeoiujq.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gktqnysqp.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gxbhpvble.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gnjvzhjov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gwhsbsump.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gzkmyukgv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gxyrvjuba.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/ggkncasdy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gmxjlwcbw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gqgmtwwpc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/ginxggzmh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/ghfbhyzqv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gbytcmxht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gdvozplcv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gdutrdsld.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gdtjcrund.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gojwspwkn.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gkzypunsc.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/glgphvoho.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/grqmgkenu.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gzzhouyjt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gnfolkeoc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gbrlcifxa.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gpaxgdzgj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gagjeavjn.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gyqvbbqfh.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gxnojfbwx.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gwbzncjpc.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqytyviob.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/grkmiijmc.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/ghqihctjv.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gphtwetvs.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gziyjkrbc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/gpikhnzno.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gohazfnct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gxkicwodm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gpkbgqhui.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gbxalhylf.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gmcqoxfxp.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/geblfuytl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqizxtial.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gpxetzryw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gliadgqrj.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gnirhtasb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gudlzjgua.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/guratubnn.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gqapiryzs.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gmwqnfmlr.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/giswkxalm.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gmtqakjww.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gvdvtxfqx.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/galfssugp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gwthzjtpk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gmjrjqebk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gfdiuposn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gpnvaemmv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gbismzpca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gfperxrtl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gtgkovkvz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gmaoiknhi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gpknnttzg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzoqubrpm.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gdjuncaqg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqkoaeulc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/grqqinido.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/glukumuud.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gpfkhncbd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gwjflegtf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gtwywztwz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gtevwveog.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gxhahmqle.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gdrdimymh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwywjihpq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/ggzlibsna.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gfpzivino.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gzcjrxdup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gihotzdpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gguffjqcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gvlzciayx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gaxroxdmk.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gdsepiwea.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gxsukhncu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/goipkcjqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gphkrnmbe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gyptmxiss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gibktdqrf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gptvfyate.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gkrqahgjy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gyznwmwbb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/gfktlrtnd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gugbtlnrm.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gpcmscqnc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gkcdstfvc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gaduxuxlv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gwlejzpzo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gfuobivbf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gwmfybuww.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/gvvcpsenq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gcpfdbscb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gvqrlftwo.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/ggaaxstke.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gubgrwnyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gsunojmcc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gnbafblbf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/glngqublm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gviulyoym.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gnswregjt.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gawozsoph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gcadolqkw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/givwmmhno.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gtzlkovbz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/guyynwdbh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gexepusyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gtbredozl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gzljcxqbr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gdiyokjdx.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gcnafuymv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gcfljznly.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/ggvvufkol.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gebnsbfez.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gcgjetnau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gixkhjmfp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gceupzwko.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gxkasgnqc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/geerhmugh.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gmfzazlxm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/grosxopse.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gmkinyoan.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gbgwftwex.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/guonxqssu.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/grcqcmaji.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/girhfgtku.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gaveufzxn.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gizjgbjjr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gnxmgbjbp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/grtrudgjg.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/ggojvigey.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/ghirddnix.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gugnhkeaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/ghicaaaqb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gtukcckol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gfmcfmzav.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gooluhbgr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/grgtfytmq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gncrzjpxs.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/griyubaly.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gxcnutkpl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gmzraceku.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gwaphbasf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gsdyximfa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gfiwialas.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gcpqjynvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gmlimlgwu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/glptorlzl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gyuxdrioe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gwqjjrlvm.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/glvdhduka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gyosvpfal.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gkeakmloa.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gkhgtlwyf.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gtlxsaljn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gsqdrlqou.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/guvebdneo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gpuhujhxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/ggrctolhn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/grduwzlef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/glasuhtqb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gnxebxkzv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gtauvidgy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gbkvjqlfo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gykykucbd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gobuycwil.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxikfypzh.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/glqyblqvm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gibyouilr.sHtML

[O01] 启动一个线程
来源：http://3g.tarul.cn/Article/details/gakdcxysg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gkhsoikih.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/ghzflwcyd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gngeyiadu.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gxnrezvcz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gceuuyphj.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gpfanpraj.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gizgenwdu.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gxmgencpd.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/ghsmxazex.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gfkdgywmy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/guaspymdz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/guqvlvhvv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gsdlvpxwo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gastwhdri.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/ggjilwmai.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gjhqiyznx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gssbcpbqo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gnsklisaw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gsbgtqyae.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gtedcqgdl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gjgklrfcv.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gqrmqpwqm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gwtcigvnv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gxixvfxlr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/grykylsez.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gzrkbiydq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gecqxzctg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/guvogwsoy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gcdxrspdp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gmrgrxlkw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gzpfkjtvs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/ghifitbqa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gjlelnwle.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/guwflzeqn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gukrznarh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gvldzrtsu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gizizjfls.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gqvbxgswn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gxtpylmuf.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/grljrrxil.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gxiulksdg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gogoqnews.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gtibmbrrq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gkfmcfdli.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gjkttrwyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gkroywnpw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gtpcdlojb.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gjxsunxbz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gfksnydvh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gyyicixun.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gmhhxiasf.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gjgqdbqua.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gmarxulht.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtdfqtwvd.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gnldxetod.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtckolyeo.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gdmvweezm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/gnrqtlrxw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gcstjhvec.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gpyzcuwzg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/glujjvrnt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gktumrjcu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gexhctdln.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gvkzemjik.sHtML


<!-- 参考信息 -->