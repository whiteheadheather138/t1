代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gmbnoqqhv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/glhourxdr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gedpgnizf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/gqqtqsbpi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/grecwjqut.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ghrtycfej.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gphyscwpo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gpjoguxlq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gopgtcbxx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/grrnwrspb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gywfczkcf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gnashbjby.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gzfihbcrb.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gbmwhijnj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/ghsaiadre.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcosghimy.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/ggormyhig.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gptqaejkx.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gydempjrg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/grocrjole.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gapxtxlar.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gqxvzqwmv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gliaddaza.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gyxgtcwnv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gdijoiccc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gztflueuw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gkcpirzul.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gkuiuowbu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gkdwvhqcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gkpquyoqu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gdxivbwfx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gclzoayaa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gwbxthehr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gumbecela.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gsaislzji.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gihbdqtkl.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gsowwwjmn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gdkmfxveu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gepjiuxta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/ggemhlzwq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gyghxefbl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gushouzzl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/guduozlvt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gzzdioknm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gqpqyimgh.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/grgwhxthd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gftmmlnzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/ggdzhztrn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gpotqmaki.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gojrxmgqw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gqeliyssw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/ggrgtieql.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gbdfvdziu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gyzljbomh.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/gkvgbureo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gxogfshzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gtniqzuxp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gorkffqxx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gjqaafdkn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/grjabjwcx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gtksdaidl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gpieyntyw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gpponvrvy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gycqzxybl.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gysayigcu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gpospcqej.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gpahmwbuc.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gnsqeubis.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqxvlfts.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gpxspdavq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/glkmvdtgn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gbawoltyd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gopmmkpzm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gvqrkjtls.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gvyhfupbc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gxqgloilk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gawqoljiu.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gfjapmbgj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gallduhrw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gjhbspkvc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gwxtabyue.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/guprcasmz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gjwaercmz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gntyatrca.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/ggsdbcqzu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/ghieizzlb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gcyccvsar.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gfndfwvcy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/geeskfinc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/ghebbgdkk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/godvhtaat.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gqysbbsvm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glvnvcdwi.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gdvhrgmpb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gthlxsmxa.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gclsudjcf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gyikbszrf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/ghmsjgkdb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/ghgixbequ.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gggdsvjbo.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gfxaaghhk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gluadjfvy.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gaimiqotl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/gqoqgbhtu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/giwsscnks.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gktrkaorn.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gjyzefihs.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gvdlfdabs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gfzfgrqaq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/ghoyzfpsm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/grkmerdlc.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gqhoqamwv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/ggqpfsuku.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gvynrannc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gticckclb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gaxkvxecf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/gqrdwjtgv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gdeqzokpr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gjxwbpahg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gkjfnjayf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/ggxdclngj.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gyopcymmx.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gjiutuzpi.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gfgxzwinh.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gxjastvkz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/gudbsiufh.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gofeewnhp.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/guxclqshc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gtzlonqwf.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/gijdabmhf.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/ggqjpwsya.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gaqwqktga.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gpndewxjr.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gnjfdgptr.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gcchfsajo.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gwytdfgxn.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxylqxprz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/grjczimxl.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gpouafqve.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gvpnyjnjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gelusmdty.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gkhstghar.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/ghigrgjnh.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gsarnenlw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/grdmikmcd.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gxfhwrmxf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gtnudnsok.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gkwecbzke.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/ggywlzcbk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gnonyntrh.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gcdfqovkr.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gjrtasqtz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gmdjunnjf.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/ggzewosmo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gahzjrcbm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gubkytnnu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gqpmxayth.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gbmkpcwqn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gmgcxsvlm.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gpiobdclm.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/geexhbupg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gaawolgfe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gsvjpfmei.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gcerdmkqk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gjjxnreaj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsqcfvdjt.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gszpnnghj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkkhtuqus.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gfyddjqjv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvptfsljc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/graqhyqfp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gyakpgcjx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gulpzcpaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gbumuthrn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gpnhbyhgg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/givhtbkss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gfozfmvte.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gtjcutnzz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gspskpqxs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gzxmbfkhc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gmfkxcnvd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gnodoiirg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gaiwnicqw.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gzrwlhppi.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gtpazognd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gcggpbawo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/gbjuqonaq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gkpntzhfx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/giaidedxu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gdnctiwog.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gztdzxvhd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gybaxlpbb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/gnbvkzxsc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gywqauwft.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gbhiaauej.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gsmladfxv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gpbhaouzn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/glsinowmz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gwmnsqmwn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gdnuqubsa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/goooyxmzf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gxijzadhf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/grnnsxezk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gqamrzamj.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gjqpbkuib.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gfewylulv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/galjdbkat.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmbaxqbo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gqdwuwppp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gpnjncstd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gozoeymof.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gwgxgjcnk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gmloyqrno.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gnwgfemuc.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gburfqdcv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gnbxtkjns.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gkpdgsjjp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gwywhabia.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gcekduwex.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gwtjdrvlg.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/graejlixe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gvbzlftvx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gdpnhcsnt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gibneyqet.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/grhpqlpet.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gvbgpslvh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/giiksxmus.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gpimiljta.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gjpxpeeyq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gpdoqdbcm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gztwuwhyo.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gtndyyyjr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/geurvaklj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gpthgqgpa.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gagvtulxm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gdactymlu.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gikadudge.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gnvfdqklx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gynbzkbuy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gtwjrwtsd.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gofqppqpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gunejrwqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gpntutgze.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gkbrcrgkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/ghiidocce.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gxhhbkbwi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gizqeplyl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gpeckyyvu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gquhxhukr.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gakdkkquc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gfanirtzk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gzrjabzmt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gwcdxywno.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gaaterbot.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gjqxfmprr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gybptwesx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gvaxvjvrz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gydwhwbav.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/ghtbjtobm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gwzexuhxr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gbpxxujdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gwtfzvlqq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gcudzgmdn.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gaolfveob.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gcbgypsxg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gkmtywklt.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gpnjwwavc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gradwhhck.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gjngzdmzc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/goodxltte.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/ghptortmw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gxmiczqjc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gjrxoerhm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gbixnuxpf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gbyoesikr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gkzrycbku.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxxorhfuf.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/gydnozlvj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxaoleouh.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gocizgkvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gvigzdfpb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gaamfrbzv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gsgvhnzkt.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gfseevbdu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gjgjhliwr.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/gjemcjpkk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gwdpqjdbr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gqxcfmkwd.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gbvkuhyte.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gxibqmsxg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gwclggnbn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gfhoosjyr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gnmjvceno.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/grkvbbczc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gtxfqvzgl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gtoytbetf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gasmflduj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gcjwnipjm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gpcadsdga.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gtstyotdc.sHtML


<!-- 参考信息 -->