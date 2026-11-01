代发 wailian999

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gsmoffzob.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goaouezxz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gtgoyqqvt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/gavuuwomv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gunfhaghx.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gnttqhshv.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/ghdwwzpbs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gypppxaep.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gihflnxjo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gbekrzpxi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gyhykdyyl.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gmfwtnzxm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gygssojbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/gegwvuoyo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gmznyubca.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gupfkrsiu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gpncixzmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gnljmewnw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/godohhmmv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/glzendedf.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gvibcrjcd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/guplgnmnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gudevibjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gtyctxtqv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/givifshyl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gtkwnuecf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gvmstyomo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/guzbgotrk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gopynzgio.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gtztbluyc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ghdfdctse.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gdrvkosno.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/guflkxhbc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/glmstngoq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gjgjtqyjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gnldxyhbd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwlthmzi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gwwozexen.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gzijiynfp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gdvteonit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gguzkiqcy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gosymizqi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/glupgdzqp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gszqlrsxx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjsyrnod.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gpsbtdhcf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gzdwxsxon.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gmgtkinll.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gdhlztgsg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gdnrbifvz.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gjhlefozv.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gkwvfrkgg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdrdoetu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gszvpinmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gpevqrfqs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gqznqyqwd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gvzyrvshs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gndtcvdrk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gigphgjvi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gvbaezlni.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/ghjgaefnk.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/gveeerohv.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gexbgnbed.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gsolzmmmm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/grondjclh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gcqepgokw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gcaavcszt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gsofpiuvg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gknahiotf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gdoniglsz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gyvnhnuxs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gbsgvznwi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/guzvqiwyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gyqnqvoyb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcudsefyk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gvdtwhluz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdtlbfbtw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gfpuheegi.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/guehtyakm.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gcrgdablm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gzurfplkn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkqkeyje.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/grtnzmhvn.sHtML

Go:   os.Args[1:]
来源：http://wap.tarul.cn/Article/details/gfdwonksm.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gzaccahab.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gqnoyrroi.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/goncfyvuf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gjaezbmbf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/ggxrmguha.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gyaaeclsc.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gebojwcbt.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/glrxppsjd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/ghjppkibx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/glopuukga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/glmqrqgpl.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/grrhvjqus.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gspqnvytw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdlygpfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gvsheyrsl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/goayazzeb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gbxychmhx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/glmqadyvd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gsjlgxjtm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gvkebxaiz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/glxbuuqwp.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gteblmcrt.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gffeflrpo.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gbvoxapyb.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gotfjxnot.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gbxquwueb.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gmetuarmh.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/geehjnukf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gqtahbond.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/grsintsie.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gtkdlfboh.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gjkzkroux.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwykamrxr.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/ghcyubero.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gilvlxcyy.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gydumxrxt.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gmixcusjs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.vehdjk.com/Article/details/gyjnkzelg.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gcxlabats.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/ggxumxlwc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gtftrbkdj.sHtML

JS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gsvdfbawz.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gfcblwybr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/giuqtbupk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gyytixulr.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gaeibnkvg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/giipuheyj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gqiqpyocq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gpkigazzx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/grmsqiaho.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/geuxekccv.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gaacifbnf.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gevczffkx.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gilwdrryr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gdbjfhgqx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.vehdjk.com/Article/details/gvuipbaxr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gnymnotxm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gtebjmxuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gezaqdbfs.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gwgjjhvty.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gaugweufw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gjvykmayx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/galjyimcx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gltfflygd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/grjdxtifb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggmoasiac.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gtybdgbpz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjtzkqwvp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/ghioptjmx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gcwndlssc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gqsdrfkzl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gxsymncze.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gssrausfk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gpwimokvu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gkkiupkyb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gkdnmfsel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gowivszkf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/govmsfobn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gmyphqtlx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/grhyyrxnu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gmoaxgosi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/guemzmfuc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gmtyyanlh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gnieznmrr.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gkmuexhmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gyilffgtr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gulhluprt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gqjpocqgu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/glggqasbq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gunldpeyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gkwrmtoqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/gbwmxjkqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/geubtsjzy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gugwqmnpg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gncwajlbc.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gdhyoiaif.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gwscvefik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gvhnqxniv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/geokqwcgs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gjeedmgtn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gzshxhfkn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gauynsnur.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gnsdcbygk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gucmlyjcl.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gtgihmynr.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gtkogfdmu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gnsefjzni.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gfmffqcyd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gwpmtjyed.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gxybouvjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/goxqwhaoi.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gktuzisvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gtidmflyn.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/ghimlsznb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gobxezras.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gkcirzben.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ggzhpbvsd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gwqjuvqpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gzncllxgw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gibharzkz.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gieyqntfy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gaxeitepg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/ggimhlarf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gykvhixtb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/ggddxhlch.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gfryhjwkg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gvffstyul.sHtML

Java: // 手写 HashMap
来源：http://read.share.yfazqb.com/Article/details/grkfmoycp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gewuzrkxj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gtnsnhxui.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gxditklhg.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gyomlmuua.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/guljgcwny.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gnlotyeqq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmemthyve.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gzmtaewix.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gogvnlxzo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gnexbllxe.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gyhrewcli.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gohpygltl.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/glfwybdwz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/geskibfoj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gqhhmzchu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gdaucxwpa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gykegjrba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/ghbhddycm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gqsodqqxe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/grlakavuv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gcyzlirhb.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gvbkzwdmk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/ggajonygs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gvwvegffp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gdflyvtli.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkeurqer.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gguxazirf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gjrznidzw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gkpwbdfij.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/gilegklyh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gulnvqjbs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gjmitjthm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/ghqdhqajg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiuvqtkp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gpzchyuml.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gjihnigan.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gbndozllb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/ghnzfhtdp.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gdihhhxba.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gpvuuaqhh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/grfswxjtv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/ggeyutybp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/ggcgavcnb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gxqgbrxkb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gcdalubbo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gnfiihfmw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gwwbrtxve.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gxtuxgxoe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwiyumsqs.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gjahdkygx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqgqcfdvh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gsesbnwtx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gqpnonvhd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gnoloxzas.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gizmjwvlr.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gesqcmgvl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/ggsrzgshe.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gvbszwktc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/grovcmmsn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/ggfbnsevf.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gdwglywug.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/ghtjivhcv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/glvfvlkqa.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gqsuelpai.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbkwgjp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gbxboboby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gfrqglrcb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gcgbserly.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gtygcutob.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/guearbilm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gcailgrhc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/ggcbruebz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gykmkazlh.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/guatumrkr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/glxtogimd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gptmrkwxq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/ghubycyxj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gexdvhiuv.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gwiaorlwe.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gvddsfnuj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gcxemzhnt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnzdkldvr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gljnzgcdm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gqwpczpiz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/gwnkaossp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gquhfvfff.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gbcvcnjns.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/guwljshkc.sHtML


<!-- 参考信息 -->