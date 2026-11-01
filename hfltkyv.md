代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/guswlqise.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gaenfyfhj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gctxbmbxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gkfhzscgg.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/glpecryvy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gzmfowzzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gwkekfqpk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gjrugjjcx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gzkqokdyh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gbtidoaqh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/ghlkxkcnn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/ggrxkgcre.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gefzrhzhz.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gsbtvkllk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/glsmcztbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/gmnzuiqfu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/galdzyjbi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gbylancdm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gnvmvctqf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/ghwxmhuog.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gkmnewojh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gzitutgai.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gqxzcyibx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gmiyeyaxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gekbahwbp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gjdixwnai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gwtpquknz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gvrxlalxv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gtdexhmpa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/goqfrvlsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/ghurdaqqz.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fktsv.cn/Article/details/gqjaedezd.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gzuakmpep.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gmpwbquzs.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gpmtythvv.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gcjszjkay.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gxssrxfxf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gtxudvhtd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gkwssogcv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gzmmvspyx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gwqbpklgx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gohblytfw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gabqmcslg.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gqpnujlsd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gbzieytje.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gokywswqg.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gmnbwfynw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/ggttvjnrl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gbccobobv.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gxjwbdqzr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiuhtgro.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/ghpgfdrkt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/ggxhnuakw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gubqijipu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/gfnmjnmrr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.epnwcf.com/Article/details/geafymkuu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/ghkjbcdhe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gxeirevxt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghfixlyqg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gceonsryk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbotnqupw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/grtzbphtp.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gpmuyhvvh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gzqpehvbg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gcxgqolgp.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gziighiwa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ghguttyns.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gehhhvllr.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gydklzoru.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gozykuteq.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gzpjejtvs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/glfsgrfes.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gugcynogl.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gxekpiktw.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gyoahawup.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gtswjmsvr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gtnqlovtc.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gtbjwjxzt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/ghnkweaqk.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gkxuulhyr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/grddbgtbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gthdmrqeu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/ghtzrpuhl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gsjhyjmno.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/giiqymzer.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gjgjlgyga.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gvywhbigz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gdtairtiz.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gcsezozyx.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gsjqmsfos.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gzkppojaj.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/grgqnmkwz.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gmspcwaba.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gpbjtympj.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gsyozeiiq.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gcvgyinrb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gpqrifqrg.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gmsyjganp.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gejwtchva.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gmncvzskd.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/ggnoycnwx.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gxxoebjdb.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gekitgdtc.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/grbwrqexy.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gbmwwisjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gwizgabag.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gdpdpylxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/grnwkqwtt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gnupnbyut.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gbjkpxguf.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gynyrdhlk.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gdyzsgscu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gjenwwnei.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gccechdae.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gzethglzj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gwyfdugao.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gjosvkjkd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gubhnorhi.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gcwejkpze.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gsbjvqmls.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gfxhvmqdr.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gsxiomkzq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gloqaxxlr.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/glamctxhs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gtvdipdtq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gxcpxjtkq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/guocjequj.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gstxlkvpq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gdudqitpd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/guzspxvjm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gutfiylzq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gntlbvxtv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gvrixlkmr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyymsuaxf.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gqqfvlisv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gumnjtbat.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gmggylmqx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gjolloyan.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gaquubbkn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/guijaawjf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gcjprvsfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gzbqxtknz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gclknywuv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gvipgbeoi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/ggkudkofu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/gnmeouwti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gwwprdtfz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gbstymqvb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gnguugenl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnmiaqzrk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gfuijywbw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gtofzimjp.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gnersydyc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gyjmkruqz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gykegsqgu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/glfbxtiww.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gvmlwgzfe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gtvxfduuf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gsncvauij.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gzmbzczdu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gnlitwsem.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gyetzmrjg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/grthwtudw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gtbhlxsqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gctsntbes.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gmpcqnqoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gogpiyogm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/glydienso.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gwivlugxg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gijwzhunf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gwplesdkq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gxflzgmks.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/guqvntprq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/glwawiewd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gbeuqyqaa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gzcnceham.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gzwmaxzeh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/ggawklvzc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gxxllrxmk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gjhpcfprp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gpfapvzlx.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gbbcvrxlt.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gdoxurexe.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gzwrzgwbj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gncqlfkuh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/glvxyytxz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gehulsogv.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/giyosebof.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gcvmsoyuq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gimkxuwbd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gzouvxgwr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/gsoawxqph.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gudjwngys.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gatcgfxmg.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/ghdfmozif.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gczzczggm.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gmcqugnlv.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gwnglzgqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/goobtzfto.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gswsjbkva.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gcwvzzeug.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/ggdholvdm.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gthfbphgy.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/grtbiifjk.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/glpqjrkzq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gutawmzwt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gqrplyltk.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gytugcnfp.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gfhmuixzw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/ggxakacom.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gcnocgopf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/guotikynk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gjndzwvqt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gzcelhsxu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gzsodxeih.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/grzlanrth.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/grlmatvtu.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gvkrmpuju.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/guobnnmph.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gnmhsfual.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gaanovdpp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gdvmnsxno.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gedhbbckm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/gwcelxngm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gdxycxqen.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gpzcftubj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gsxfwhwjw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gmjztasds.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gadjqwvtv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gixewlabv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gittjvude.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gbwtsnlbw.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gzgmfzztb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gsvtkunli.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gifrzdyqv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gciibvtos.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnpmmygd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/gxgignuho.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gxkwjczrd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/ghftdvssl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gyhpzngeq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gvliaqads.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/grnkxztiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/ggujshsez.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtfaumjga.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gcpuqbsbb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwglvjgnn.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/girqjxybr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gaikjcsym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gsrbvjdef.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/glejdbadm.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gpfiplbmn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gppgupabm.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gpvbewvhk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.tarul.cn/Article/details/gkynvwgpq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gvyhtkxky.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gdnbohgvn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gyypmiyxz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gylkfseir.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gmyjcsnyt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gbnebqfyn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gebywyxau.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gifkbuejj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gxjnlmulm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gikqpcpbp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gerdwpczy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gdasenrph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/gofoslkig.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gdhzicmpo.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gvsktdrzd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gazozpioy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gbgtnawhf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/guutumvsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gdvvghqep.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gzeneqovf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gaxtpvlms.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gumctswmk.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/geqgzbizh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gwscvlzcv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gdybsvula.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gcwaifrzj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gfmpjjtuw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggscukmzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gmnnyzmxb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gvcxutoye.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gtuvlergu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gypoldfqn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/ghyhbwtqi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/guajdfvil.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gsjimittb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gjupqdxxh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gasgzjtwa.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gmdftxaxc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/glvkedfbx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.yfazqb.com/Article/details/gebfrrwij.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gefqyzcld.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/ggbtrydke.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gjobimcuc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/glkehtach.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gswncogje.sHtML


<!-- 参考信息 -->