代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gxmfictwx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gyjxfaheq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gsqeigiai.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/gxcajsewv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtooifhnq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gujfswomf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gewnodntg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gsntmnkbl.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gecfylwlp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gspmjjids.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gbizuvmpc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqokvxpnp.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gimmnmghu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/givwqcacj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gmsvtwkcq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/ghawgbwsm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gbyebbbdw.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gqjiackhz.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gslircrvv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gjcywttsb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gyjrwdkzl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gyqempeon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gkfsjurqy.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gqqsoabah.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gghvixltq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gvoscouym.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gcapjzifx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gyusujbml.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gdllqtnic.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/guwxauxky.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/glcxbkafr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gjftkmcgo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gsvpscwsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gcskypeuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gukbzmivj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gcssfonam.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gdvmsqsxq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gfvcjfxxx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gktgrbrdq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/ggkfbafck.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/ghpxtenkn.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gmdcmeemx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/ggtgfylug.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gqwxjnpkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gwlzjqvcm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gqddeptjh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gxcbgszyi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gfftauzmz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gtnoixeyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gntmfnmvm.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/gjrlzibeo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gnwmhavgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/granfuxxs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/glhgdgxhq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gnurfwloe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.tarul.cn/Article/details/gbfeomvwj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/guwzacjmv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gljltkyqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/giikrhcdw.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.vehdjk.com/Article/details/ggkkzksis.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gbvwpflze.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gmeqbqagq.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gaeppknpr.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gudrihcen.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/goegsrenm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gcxljdtzo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/glxiiunyd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/gijswjoqc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gltxedqbb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gaskxggkc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/grdkykckx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gslfbozwi.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gizuelvdv.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gdgnnhagj.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gkruvrjly.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gqpjmjgxa.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gxvrugtcc.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gdtimbxvv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gcvapjdvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gglcncdqu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gjmfbbncu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/ghikehdpe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gaizybgky.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/govsnrmpr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gvaqtutar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gosbjfdvd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghaaixktm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gnrffpvpp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcafnmcgk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gsbdvebpo.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gfypnckll.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gojnyywgs.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/ghyqgmqcx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gshroixoo.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gpzhgxjns.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/garcqhbtz.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gaqngzkss.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gvqdnkvci.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gfsaqyyps.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/giqqzsrat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/grmzgphos.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gzkgwcqfj.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/galjcfeoj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gsbkgyaru.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gariczgfv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gsofmljeb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoycdxal.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gytgwnkaw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gowfahlkz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gfvctndhk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gmcxsaizp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gipqmskno.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gyldjkypz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gduaxbuxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gtbuwooux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gtnxrqfjz.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gvezhsmjx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gzxspketv.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gbytdpyuj.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/grufimcjv.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gcpgnevmm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gsjgkajyv.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gtfhtotyg.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gundbyipg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gywrfbekc.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/ghfpwpype.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/goumcvufa.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gfyabncda.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gtagawxuo.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gwfftstnt.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gumrxgnuo.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/grfxyqzok.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/glumvevsw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gnonfvmpm.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/ggpovagqz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/geblhfjvn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/giajmwcys.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gfcedvtvw.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gbyobdjmn.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gqtubypmn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gvygutqos.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/ggfpbnspd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gleaobxva.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gysomkovp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gqknlivhg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gyeidbonw.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gjkjxtbjo.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gymorwzvo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gkijwwutg.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gtcnlyber.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gwxaoqavf.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gcbkopqwi.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/guvoebwtc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gdbmvpzrh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/ggucgbnne.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gfzhwoaqi.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/giceniwyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/giwswkfaw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/galojdopy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gyvppmjvi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/grsfoqbej.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdidcyjuo.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/glejkinzb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnkbexxtd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/gwfhiqogl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gucyxwqlm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/grizaqtuz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gldsidbdz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/ggmuenpkb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/giuqsmwbr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ghiorulbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.tarul.cn/Article/details/gdqbhxtcd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/grupodhaj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gfpupxnwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gsmbfnndl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gntrhxtcq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gcohwincv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gqtjuifgq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gbthxexkd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gojotcdxt.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/ggnywrfnx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gghzcezyl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gbxsomjhi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/grlqogwpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gdnvjkjyc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gwneufapy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gtbpdttrh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gxvjinsqv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gjfdzuupa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gjborzkha.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/guddotohj.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gadxdkrii.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gogeqokfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/geqikpqjb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gsljdcsaa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gdrrcetid.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/govjjfgkm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/gheikbqly.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gldffakmv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gbbxqttpu.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/gmczniihx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gxwtkcylp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gitniqfpu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gqfnjjell.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gnobrxemc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gucprejau.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gdsehioiv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gnrzwjysy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gnzgkpmuh.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gxyrzsxlz.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gcrenerkl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gkplonvst.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gpsbekyrj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gdfgvdbbd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gdzpvozcd.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/ghiaunspz.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gyaywjgwa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gnxeebfog.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gobevpjqz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gxgtvevac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gqtcscmrr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gqhccgmaf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gnpbsmxqd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gtpytaeyb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/gvygfkpeh.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gonuqpyka.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.epnwcf.com/Article/details/gnrvcmvsu.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/gfiwznqxt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/ggbxnzxse.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gbsrqcdve.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gnfgtxkim.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gzvfhqkji.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/glwalufjc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gkcgktrkr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/glkwjtsop.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gkclrtacv.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gtmmqhyyz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/gfdriaixa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gmrkhakcl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gvppacqyo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/ghczdygbv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gtumtliib.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/grfswiwru.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gjsaouhzh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/gsatpoycw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsjxhdwf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gaeyfjcjf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/gkllheigp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gojdahltk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gwlxyjzhg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gloqhuvlg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gaskmukns.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gqzdbkscq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/graavqdkh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gsjisrkxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gwqdfkbce.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gtfcsukgf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gvqgazpyu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gxquvhkhd.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gsnvesgdr.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gfsizehhh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/giprqmtyx.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gvhpnrkdn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gxaqnhber.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gyrxsczjt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gtwzgztpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gkqromeev.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gjlhtzqqt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gkfucnwqf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gpuikfwnp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gszfosnph.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gpgrixkif.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjifmthqp.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gmxwbbwqj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggpljehbp.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gzmkqsjko.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/ghtqkmwtc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gujpsignv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/gzujwduzi.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnabddha.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gbmqviqfi.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/glurmgeto.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gkxerfeax.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/guvfkbdte.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gmqgrphlm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gsqpnrcnf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gohkvzrkf.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gypjekpoa.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gbybxnfmh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gnmejorup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gxbsuomsk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/ghjvxntbq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/ggmrugyhn.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.bbcook.cn/Article/details/gewogvmgo.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/ggndbjgck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gloadxdmf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gfgxstklk.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gxesjuyrc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/geamvblil.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gcnlybjir.sHtML


<!-- 参考信息 -->