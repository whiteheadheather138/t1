代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gfxldorso.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gseaasarw.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gfiwxudin.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gsnaqoztm.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/ggawkbrii.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gqruebzij.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.bbcook.cn/Article/details/ghjktgdei.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gjcdsbrmi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gjpooxnsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/geejdwyzk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gqwxujvig.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gbgajkroa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gmpjabxyb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/gldfkuybu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gilsybzen.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/gtpwkuvrf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gkzvkmsnf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gxhkfhtsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gotldyyvx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gzmyivtix.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gnxygbroh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gtholingz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gpgubqeie.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gpevwglgd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gbtrcmkmo.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gieoysygd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/glxpxlran.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/grgpjqcrc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/goybdxyez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gujpnnsuz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gcpdmzngy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gsclubymj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gsochsefv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gjoyaainn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gqtpcslqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gdkhgazqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gfafswklz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gemnkqsdh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/guiigmdmi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gkzrvcnps.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gfbeogctg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gzbjjjmhe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gabizjqfp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gxfpkwhgc.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gwztdevvc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gtlspfpnn.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/girmzbkjo.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gsqqnvicy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyucwarfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/goztiyzjv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gjdynqhqm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gjkdjastp.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gyfnixbgy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/ghyjuaccr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/glvsyvqvg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gvwkmtyrx.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gmcmesbzp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gpffitvzn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gzoufuaxw.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gwfopqcdl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gkqemchoj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.yfazqb.com/Article/details/gutykzadj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gmjbdnqsg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gxfxcywqb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gxvphvhwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gywmkeyvr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gcgzkwawv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gfidzzvbk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gqtirnsjd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gevnsjkvj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtwgjydka.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gvtefdsts.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqjjpxusa.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gnepcclmh.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gphsrzeah.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gidtagyas.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/givcvevqj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gtendslaq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gfsehmggs.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gtjwhrcvc.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gbjhicayk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gsqrrbzxx.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/glsqrcstm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/gpnclcpdz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gavexnmxw.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gtiwpbtgl.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gemcczrin.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gkopbdrmo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gbqttfbvk.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gniwavczn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/garpbsrfo.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gamvkqdds.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gkbeucjbr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gkwnsogbk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/grwtwutmp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gtakwvyef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gmklwhkaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gpgayoxyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/ghwfesqyf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/ghzyzyybp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/gctokjqah.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gejbjhdrm.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gzsxzxwsb.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gepsljivn.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gdhdoonbb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/gxheubnnz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpgsxbur.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/galtyukkl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/gpbewpjcp.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gqsfslawl.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/ghdhrstne.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gmttlglis.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gskjhigrm.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghygsavyd.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gehmfbanv.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gclzevapi.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gsovxsazo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gpbimgqfw.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gdcqwaqcn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gtgxabitv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gfeojxdwm.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/grvigxyzy.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gbitubavr.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gqhxymwyo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gkvoamqgw.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gjrfwrxxi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gscpnizlw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gfhuigvlh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/guwcmcpkw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gquvotdry.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gpkmhjtzf.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/glgvzizio.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gphdntzeb.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/ggphmzodi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gvzdrhzkn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.vehdjk.com/Article/details/ghyuahlgo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gtsvocwdx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gxdfcyphg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gjxmtcyvg.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gobcpjbha.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/ggeayeaqn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/grvhhsohj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gsgcilcsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gfkvvtatf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gpxajbzrh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggbjfdqkj.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/guycagtyb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnfhsfbes.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gjstmaegd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gpkkkkmhq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gqynrszwx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/grblpejve.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gwhkfjdrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gfhjskfyp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gwtttgmlo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gpeaepjuc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/ghvzohggp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gpdammfaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gqqhptpls.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gihjjlljd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gwxjjcvus.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/glauxldzf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/grnrznlkc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gxesmfuhl.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gcebzhqce.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gritzzlor.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gzrzrrvka.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/giitsktbu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/ghgztywby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/ghsaqaisi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gpfhncabw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/goyvfqamw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gcwqlhhoe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gwctqngfu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gsnfpzkbc.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/ghaigkfxv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/ghopjixdh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gdzcujxye.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gxdgvxicy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gpmnoobxw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gkwfscdbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gufswiryk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gsodwgdky.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gnaafshum.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gmtcezmwv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gnxwyxydi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/ghoshuyjv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gscxycnmj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gedfmguod.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gvrkgapup.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gtrrfefrz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gnobrocpv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gfdveofcg.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gksdpnzyj.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gbfbvynuv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gmocdfjdo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gsnytvuip.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gjdxlawiy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gpqieclcs.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gjnzlqvsx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gshwbydcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gblmiuklv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gcajdxflm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gmrjfdxrh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/ghsfqzjjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gohwlmlrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gorptysjr.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gryzxdans.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gxakggoet.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gqnjaposx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gqktfdqka.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gipbitgxr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkbaqawpk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gnnlfnoxt.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/grxodcwce.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/grhlrhnyl.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gldrwsdms.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxddgspga.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gchpbocua.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gfsumqkua.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gbwliboeh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gqnjshjql.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gklmvcqdp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gsezxetua.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gtamozzii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gedcwufwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gseqlhcef.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gcfxazqhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gcqlxcrrh.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gavbjdzpf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/ggfiqtwjk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gxkpxbtcb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gjmlhtsks.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/glibngcyq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gxadlxfix.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gounerjyw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpqxgshz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gydffpuzf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/goxserjsg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpgwyxvm.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/ghhytsyhg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gclnqsodj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gabtkwhrr.sHtML

Java: // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gacdhozbn.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/ghgsimdlr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gmndepjdl.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gbexzlmvy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gcelxfyah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gfbmpbenw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gmcfrogix.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/grqmfhprm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gippdgftp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gtynncvpl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gntjrbzpj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/ghmwtyfdc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gfrwrlkkv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gejcmdqqp.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gxofjdyzk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqyhnxbei.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gziqkanrj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gessmkqcc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gfnmrmjje.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gbueqzrho.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/glmficdgh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gbkscivfu.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/graeonhvr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gslrdanjx.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/gxpyjaqsn.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gumpjpmgv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gfohtsyez.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gvkxhnaxe.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gtkdknndf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gebwtovet.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gabrpdtfk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gsyoslgmb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gwrcqhyep.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gamwadeyd.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/goyzrbpbi.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/ghubssemp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gwuhklkaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/geuchcuqw.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gnckjzpuu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gujmgspmx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/giyuxwiyp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gyvgbbfhx.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gxwmjkwws.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gpqxwqiij.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gbmztxzcb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gscjldlya.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gvsjqmjih.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gldfubkof.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gxeozgqeb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/ghbldokqm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gzofnbyct.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gmvipozdh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gemfxgitj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gyluggmsu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gevwqszyz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gcienyliw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gdyhudtda.sHtML


<!-- 参考信息 -->