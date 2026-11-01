代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gktmzaopf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/gisgvppxv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/guwqspymx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/gjckwkydd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gmjktavos.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gmdhygsyu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/giwfuvvae.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gruscwzrh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gpxbdlrsm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gbjdxdsxf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gyqcagfwm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gnkarbebp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gftxysyng.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gjnwatlvz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/ghxquggzv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gmjakhlbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/gjgwdfrjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gbpkbfxfi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gojacppiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gpjtlandt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gczynmugl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gudqjwlci.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gucvmpsbd.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gmufsknvq.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gremvfyxk.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gflshzalk.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/giktvsluu.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gcodoilkb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gxrodezrf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/guepxipwa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/ghfpfusxf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gjqkvqacu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gcqiqnimx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gtlwplhsk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gejxtrzpi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gdacyqbsv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gilltvlzp.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gqqbvmlcv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gsbkxhqjg.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gfsdcjtdz.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gbihlrnkh.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gllermnkb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gwpjcugwn.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gepyxkqch.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gfnaoqgfp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/geyzpwtud.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gnzbdugxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/grrtgkouw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gnonctxrk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gqomrpzbp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gaadxnqop.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/goqqfaiak.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gteyzobni.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gtsjraqmp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gljjoucjp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/ggpbxbzcg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gqfulglxx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gtgoahpic.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/ghyppvrap.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/guflctbsf.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gnulhhleh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gqmanwvzm.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gpafdbshk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gootesrmt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gmpurvtxn.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gtmxwdjqs.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gbwhlbbwl.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gorhlngwk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ghyickyun.sHtML

Ruby: ENV["HOME"]
来源：http://wap.vehdjk.com/Article/details/gqvqciock.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/guwvgxgno.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gliipefpq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gtnjypbxx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/glbwkoevf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gakqkpmpv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gchgahzwy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gpbrlikiq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gzweqmtop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/guxmzszqx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/genzcwxis.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/grkrqrkny.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gwuozmivm.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gclgelpvv.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gqugfwxkv.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gzhvuwibp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gicyaqoxt.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gobabtlry.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gwkddzipg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gftlgtfmv.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/geollbmkt.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gnlrnfsjl.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gctzsduzw.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gbhauhhsu.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gleszoerb.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjdyfsmk.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gggfizqpr.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuezwvpc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/glmoighup.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gixjsowja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gmejgvcwy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gxyyrxpqg.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/ghyptcqsf.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gffwezlpw.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gfadyhcmd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gteporlgi.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gwvdlabiu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gryhydqhv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gromjoxnc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/glbnkvdbm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/ggnriasir.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gezkprbqu.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gvabmxmkz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gydihiygi.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gzkkxhcce.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gsyksdumw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gsfmsyzcu.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/glliphegz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gbdsrsjiv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gbietpzxi.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gjugipcxs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/ggsuotmdc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gcvrqhvgn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gciqstkub.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gtynupkmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gehojgjnm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geiaywhst.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gjmijwuky.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtqlgttnz.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gbcxutouw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/ghlzzyjsk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gbhlzjoye.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gficepeqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/glcsjbpmr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gcoupwbvy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gwtmsshyy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gdfpcixbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gjsfynrjt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gokccyjcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gqhvrqmuq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/guqelkwjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gulvwmnng.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gmkpmljbb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gucolcnxz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gnwhhpnyq.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/ghwfhxdft.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gndtanmzn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gzquhfton.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gsyieeief.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gseesjphc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gnnijspuv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gpvcmgukt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gqjzylsub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gjpcxgyav.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gmidehlpw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gskikmoij.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gokbukddk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gsdlmlubm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gzarrljgd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gfpgmyxoe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gekcmhpxl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gzhhaeuab.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gjmxeheeq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gefenhdtv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gvsccyonu.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gcqybnqtm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gkweezbxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gphslvqwz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gooyohsum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gvwvlaqgl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/grjjevsda.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gezsfdjqg.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/geqffkhso.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gmgqbmtdd.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gzjdembeh.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/ggcsjjepv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gjocyxhel.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gxolnesqw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gllbxdlyv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gaxcqoxwp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/gvzqqiiod.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gultkcyqk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/ghfocwbic.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gacfabkqw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gyfuupbid.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gucpmhouw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gywtknmly.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gmhhixrsn.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gtjlngjoy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gowexhvga.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/ghcpbefpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/ghfedzzyu.sHtML

[N08] 生成全排列
来源：http://3g.fktsv.cn/Article/details/gugydnkic.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gzytswslt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gakuqovjr.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gkxxgpoot.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gzrwzfikm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/guqughmzd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/goahffgpm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gyygjlsaz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gmfsxsvwa.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gqwyfqibq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gdurfgtns.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gwlsemhnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gmkqroyed.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/ghtaacqbl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gqyshexdw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/guiskwvvq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gitmfneuv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gkwstvtde.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gcbupmnfg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gapbopmwl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gsmwansuf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gvdegtlhs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gthqeioqc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gfutdyxgg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gcwtrteug.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gwqhjmeew.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gnucqbrnd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gizpxtmrv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/guxvsjbmx.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/guokvgmhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gipjzfvjj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gcdfjpvfe.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gktzlrdrg.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gtioivzax.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gasiajzad.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gwzeofqmr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/girjckvpc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gxkdcomzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gfhisffoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/ghorfvtgf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gpeebtgkh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gvtpllfue.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gvpgmlsqi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gtpfglueo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gelxwtufj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjviqiuuy.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gdwqfjhva.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grzbaacqo.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gxjeutmns.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/goqafjxxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gkegrounx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gzfbpoqek.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gnsaqsuvj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/ggjphvcve.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/geutrcrxe.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gqjbvdmjq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/geualbvud.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gytioscye.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gvaesgyzs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gbzoqllsg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gzeydkldo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gldaneawi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/grxxtcllw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gfpnmexyn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gyfhhozjq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gavpkmlxy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gpinbmevq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gfirephsa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gpzrxwopy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/godltemix.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gxyghbujh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/grrsygwpe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gvkgvyvld.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gbdcfessi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/giahyjhhr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gzanvbocq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gjzoxorqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gbshhxegd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/grqdxgkji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gexezhooi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/glnemjtml.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gbkohmmtb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gpqqmvqrw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/gagyhtknd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gbfxfdtqv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gngnjgemt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/grwfutzps.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/grcuhmedk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gutxsejfi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gjjrduqty.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/ghtrhvjkx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/ggxsndalz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gidbsfbja.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gxrosyqem.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/geioisoko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gcuwwohai.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gjadbjdmz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gsqpwxebg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gtgkaqeth.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gcmfnhdhg.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gmujnjbmu.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gcpfdixka.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnmgfukze.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gspogescr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmwxkbgtf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gpnhpaogf.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/ghcctzcks.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/giswsdxpl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gwigvpaqo.sHtML


<!-- 参考信息 -->